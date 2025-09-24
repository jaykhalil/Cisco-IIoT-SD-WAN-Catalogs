# Cisco-IIoT-SD-WAN-Catalogs

<!DOCTYPE html>
<html>
<p> The table below lists all SD-WAN catalogs which have been tested and validated by Cisco for use with Cisco Industrial IoT Platforms (IR1101, IR1800, IR8340). Each published catalog is essentially a tar file that can be imported directly into the matching Catalyst SD-WAN release as a Configuration Group. That group can then be modified further, if needed, and devices attached to it. Catalogs come with certain global values pre-configured to ease deployment, such as interface names, LTE timers, and other service IP addresses like NTP and DNS so that the user can replace them with valid IPs in their own environments. Each catalog also comes with a PDF file that explains in more detail the functionality of the catalog. </p>
<p> All catalogs are Cisco Validated Profiles (CVP) and thier names start with CVP and some other designation. In all profiles (N) in the name refers to a deployment in NAT mode (aka DIA) where lan traffic is sent directly to the internet, while (R) in the name refers to a routed deployment where all lan traffic will be routed to a central hub advertising a default route. </p>
<head>
  Catalog Entries By Release
</head>
<body>
<table>
  <thead>
    <tr>
      <th></th>
      <th width="16%">Cisco Validated Profile (CVP)</th>
      <th width="18%">Cisco IIoT Platforms</th>
      <th width="20%">SD-WAN Release</th>
      <th>Functional Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td><a href="./IR1101/CVP1N">CVP1N</a> <a href="./IR1101/CVP1R">CVP1R</a></td>
      <td>IR1101</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting single service VPN for for horizontal IR1101 deployments.</td>
    </tr>
    <tr>
      <td>2</td>
      <td><a href="./IR18xx/CVP2N">CVP2N</a> <a href="./IR18xx/CVP2R">CVP2R</a></td>
      <td>IR1800</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting single service VPN for for horizontal IR1800 deployments.</td>
    </tr>
    <tr>
      <td>3</td>
      <td><a href="./IR1101/CVP1NX">CVP1NX</a> <a href="./IR18xx/CVP2NX">CVP2NX</a></td>          
      <td>IR1101 & IR1800</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with LTE and wired as last resort supporting single service VPN for for horizontal IR deployments. Reverse priority of CVP1N and CVP2N</td>
    </tr>   
    <tr>
      <td>4</td>
      <td><a href="./Roadways/CVP5">CVP5</a> <a href="./Roadways/CVP6">CVP6</a></td>
      <td>IR1101 & IR1835 Roadways</td>
      <td>20.15.2+</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting multiple service VPN for Roadways deployments with ISE integration and lan port authentication</td>
    </tr>
    <tr>
      <td>5</td>
      <td><a href="./IR1101/CVP3NAA">CVP3NAA</a> <a href="./IR1101/CVP3NAS">CVP3NAS</a></td>      
      <td>IR1101 Dual LTE <p>active/active &amp; </p> active/standby</td>
      <td>20.15.2+ <br>
          &amp; IOS 17.18.1/17.15.4
      </td>
      <td>Single router SD-WAN configurations with wired and dual LTE in both active/active and active/standby modes, supporting single service VPN for for horizontal IR deployments.</td>
    </tr>
    <tr>
      <td>6</td>
      <td><a href="./IR18xx/CVP4NAA">CVP4NAA</a> <a href="./IR18xx/CVP4NAS">CVP4NAS</a></td>      
      <td>IR1800 Dual LTE <p> active/active &amp; </p>  active/standby</td>
      <td>20.15.2+ <br>
          &amp; IOS 17.18.1/17.15.4
      </td>
      <td>Single router SD-WAN configurations with wired and dual LTE in both active/active and active/standby modes, supporting single service VPN for for horizontal IR deployments.</td>
    </tr>    
    <tr>
      <td>7</td>
      <td>CVP7R</td>
      <td>IR8340</td>
      <td>Coming Soon</td>
      <td></td>
    </tr>
    <tr>
      <td>8</td>
      <td>CVP1N_SEA CVP2N_SEA</td>
      <td>IR1101 & IR1800 <p> NAT with SEA</p></td>
      <td>Coming Soon</td>
      <td>Same as CVP1N/CVP2N with Cisco Secure Equipment Access agent deployment included.</td>
    </tr>
    <tr>
      <td>9</td>
      <td>CVP1N_TE CVP2N_TE</td>
      <td>IR1101 & IR1800 <p> NAT with ThousandEyes</p></td>
      <td>Coming Soon</td>
      <td>Same as CVP1N/CVP2N with ThousandEyes agent deployment included.</td>
    </tr>
    <tr>
      <td>10</td>
      <td>CVP5_CV CVP6_CV</td>
      <td>IR1101 & IR1835 Roadways (CV)</td>
      <td>Coming Soon</td>
      <td>Single router SD-WAN configurations with wired and single LTE as last resort supporting multiple service VPN for Roadways deployments with ISE integration and lan port authentication. Also includes profile to deploy Cyber Vision sensor in IOX</td>
    </tr>
    <tr>
      <td>11</td>
      <td>CVP6_CVSEA CVP6_CVTE</td>
      <td width="18%">IR1835 <p> Roadways (CV&SEA)</p> Roadways (CV&TE)</td>
      <td>Coming Soon</td>
      <td>IR1835 Roadways catalog with combined applications, Cyber Vision & Secure Equipment Access or Cyber Vision & ThousandEyes.</td>
    </tr>
  </tbody>
</table>

</body>
</html>
<p> Cisco provides the configurations in this catalogs as is for your convenience. These configurations have been built using industry best practices, observed across multiple deployments, which may be beneficial to you. Cisco is not responsible for any technical issues, bugs, or other issues that may arise from your use of these configurations and any resulting indirect, incidental, reliance, consequential, special or exemplary damages or loss of actual or anticipated revenue, profit, business, savings, data goodwill or use, business interruption, damaged data, wasted expenditure or delay in delivery (in all cases, whether direct or indirect). </p>
