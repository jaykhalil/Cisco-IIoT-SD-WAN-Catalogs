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

<p>The table below in the repository README lists all IIoT SD-WAN catalogs that have been tested and validated by Cisco for use with Cisco Industrial IoT platforms. Each published catalog is essentially a tar file that can be imported directly into the matching Catalyst SD-WAN release as a Configuration Group. That group can then be modified further, if needed, prior to attaching and deploying on edge devices. Catalogs come with certain global values pre-configured to ease deployment, such as interface names, cellular timer optimizations to reduce cellular data usage, pre-defined service VPNs, and other services such as NTP, DNS, DHCP, and logging. Each catalog also comes with a PDF or DOCX file that explains the functionality of the catalog in more detail.</p>

![Catalog import screenshot](./metadata/cg-import.png)
