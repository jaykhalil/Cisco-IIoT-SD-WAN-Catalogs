# Cisco-SD-WAN-Catalogs

<!DOCTYPE html>
<html>
<p> The table below lists all SD-WAN catalogs which have been tested and validated by Cisco for use with Cisco Industrial IoT Platforms (IR1101, IR1800, IR8340). Each published catalog is essentially a tar file that can be imported directly into the matching Catalyst SD-WAN version as a Configuration Group. That group can then be modified further if needed and devices attached to it. Catalogs come with certain global values pre-configured to ease deployment, such as interface names, LTE timers, and other service IP addresses like NTP and DNS so that the user can replace them with valid IPs in their own environments. Each catalog also comes with a PDF file that explains in more detail the functionality of the catalog. </p>
<head>
  Catalog Entries By Release
</head>
<body>
<table>
  <thead>
    <tr>
      <th></th>
      <th>Cisco Validated Profile (CVP)</th>
      <th>Platform</th>
      <th>SD-WAN Release</th>
      <th>Functional Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>CVP1N/R</td>
      <td>IR1101</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting single service VPN for for horizontal IR1101 deployments.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>CVP2N/R</td>
      <td>IR1800</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting single service VPN for for horizontal IR1800 deployments.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>CVP5/6</td>
      <td>IR1101/IR1835 Roadways (w/o CV)</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting multiple service VPN for Roadways deployments with ISE integration and lan port authentication</td>
    </tr>
    <tr>
      <td>4</td>
      <td>CVP?R</td>
      <td>IR8340</td>
      <td>TBD</td>
      <td></td>
    </tr>
    <tr>
      <td>5</td>
      <td>CVP3Naa CVP3Nas CVP4Naa CVP4Nas</td>
      <td>IR1101/1800 Dual LTE with active/active &amp; active/standby</td>
      <td>20.15.2+ <br>
          &amp; IOS 17.18.1/17.15.4
      </td>
      <td>Single router SD-WAN configurations with wired and dual LTE in both active/active and active/standby modes, supporting single service VPN for for horizontal IR deployments.</td>
    </tr>
    <tr>
      <td>6</td>
      <td>CVP1NX CVP2Nx</td>
      <td>IR1101/IR1800</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with LTE and wired as last resort supporting single service VPN for for horizontal IR deployments. Reverse priority of CVP1N and CVP2N</td>
    </tr>
    <tr>
      <td>7</td>
      <td>CVP5_CV CVP6_CV</td>
      <td>IR1101/IR1835 Roadways with CV</td>
      <td>20.18.1</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting multiple service VPN for Roadways deployments with ISE integration and lan port authentication. Also includes profile to deploy Cyber Vision sensor in IOX</td>
    </tr>
    <tr>
      <td>8</td>
      <td>CVP1N_SEA CVP2N_SEA</td>
      <td>IR1101/IR1800 in NAT mode with SEA</td>
      <td>20.18.1</td>
      <td>Same as CVP1N/CVP2N with Cisco Secure Equipment Access agent deployment included.</td>
    </tr>
    <tr>
      <td>9</td>
      <td>CVP1N_TE CVP2N_TE</td>
      <td>IR1101/IR1800 in NAT mode with ThousandEyes</td>
      <td>20.18.2</td>
      <td>Same as CVP1N/CVP2N with ThousandEyes agent deployment included.</td>
    </tr>
    <tr>
      <td>10</td>
      <td>CVP6_CVSEA CVP6_CVTE</td>
      <td>IR1835 Roadways (CV/SEA) Roadways (CV/TE)</td>
      <td>20.18.2</td>
      <td>IR1835 Roadways catalog with combined applications, Cyber Vision & Secure Equipment Access or Cyber Vision & ThousandEyes.</td>
    </tr>
  </tbody>
</table>

</body>
</html>
<p> Cisco provides the configurations in this catalogs as is for your convenience. These configurations have been built using industry best practices, observed across multiple deployments, which may be beneficial to you. Cisco is not responsible for any technical issues, bugs, or other issues that may arise from your use of these configurations and any resulting indirect, incidental, reliance, consequential, special or exemplary damages or loss of actual or anticipated revenue, profit, business, savings, data goodwill or use, business interruption, damaged data, wasted expenditure or delay in delivery (in all cases, whether direct or indirect). </p>
