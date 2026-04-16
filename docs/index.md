# Cisco-IIoT-SD-WAN-Catalogs

<p>Cisco SD-WAN Catalogs are essentially edge device configuration groups that can be imported directly into Catalyst SD-WAN. Further, Cisco Industrial IoT devices can be added to the group and the configuration deployed with few clicks, reducing the need to build such configuration groups from scratch.</p>

<p>All catalogs are Cisco Validated Profiles (CVP) and their names start with CVP and some other designation. In all profiles, <code>N</code> in the name refers to a deployment in NAT mode, also known as Direct Internet Access or DIA, where LAN traffic is sent directly to the internet and no hub is present, while <code>R</code> in the name refers to a routed deployment where all LAN traffic will be routed to a central hub advertising a default route. When using any catalog with NAT or DIA, a configuration topology should be deployed to deny all route exchanges with vSmart controllers to avoid edge-to-edge tunnels. To do this, tag all WAN edges with a common tag and then apply the tag to a rule for inbound and outbound sites in the creation of a custom topology in <code>Configuration &gt; Topology</code> and activate it, thereby stopping all tunnel formations. <a href="./metadata/deny-all-topology-for-dia.png">Sample deny-all Configuration Topology</a></p>

<p>All catalogs control egress interface for traffic generated inside service VPNs using the IPsec preference field in the transport tunnel configuration. When doing Active/Active, the IPsec preference is the same for both tunnels to load-balance traffic. All DIA traffic uses the current active underlay WAN interface. In case of Active/Active, both interfaces will be used for such traffic.</p>

<table>
  <tr>
    <td>
      <h3>Need help choosing a catalog?</h3>
      <p>Use the interactive selector to map your router family, preferred primary WAN, and traffic model to the closest published Cisco IIoT SD-WAN catalog in this repository.</p>
      <p>
        <a href="./catalog-selector.html" style="display:inline-block;padding:14px 20px;border-radius:12px;background:#0b84d8;color:#ffffff;text-decoration:none;font-size:1.08rem;font-weight:700;box-shadow:0 8px 20px rgba(11,132,216,0.22);">
          Open the Catalog Selector
        </a>
      </p>
    </td>
  </tr>
</table>

<p> Once a catalog is imported as a Configuration Group, that group can then be modified further, prior to attaching and deploying on edge devices. Catalogs come with certain global values pre-configured to ease deployment, such as interface names, cellular timer optimizations to reduce cellular data usage, pre-defined service VPNs and other services such as NTP, DNS, DHCP, and Logging. Each catalog also comes with a PDF file that explains in more detail the functionality of the catalog. Below is an example of where to import the catalog tar file in Cisco SD-WAN. </p>

![Catalog import screenshot](./metadata/cg-import.png)

## Disclaimer

Cisco provides the configurations in these catalogs as is for your convenience. These configurations have been built using industry best practices, observed across multiple deployments, which may be beneficial to you. Cisco is not responsible for any technical issues, bugs, or other issues that may arise from your use of these configurations and any resulting indirect, incidental, reliance, consequential, special or exemplary damages or loss of actual or anticipated revenue, profit, business, savings, data goodwill or use, business interruption, damaged data, wasted expenditure or delay in delivery, in all cases whether direct or indirect.
