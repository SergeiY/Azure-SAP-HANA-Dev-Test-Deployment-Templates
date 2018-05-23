<h1>Azure SAP HANA Deployment Template</h1>
<p>This template takes a minimum amount of parameters and deploys one or more VMs, customized for use with 3-tier SAP HANA, using a variety of custom and gallery operating system images. Each VM is configured with two NICs, each with one Static IP Addresses.</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.single.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploly SINGLE SAP VM</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.netweavergateway.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a NetWeaver Gateway Environment (1xApp, 1xDB)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.gatewayfes.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a Gateway FES Environment (1xApp, 1xDB)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.sappo.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a SAP PO Environment (1xApp, 1xDB)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.sapbw.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a SAP BW Environment (1xApp, 1xDB)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.s4hanautilities.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a S/4HANA Utilities Environment (1xApp, 1xDB)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.cloudconnector.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a Cloud Connector Environment (1xApp)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FAzure-SAP-HANA-Deployment-Templates%2Fmaster%2Fazuredeploy.s4hanahybrisbilling.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a S/4HANA Hybris Billing Environment (4xApp, 1xDB)</p>
</p>
<p>The VMs are configured using the following sizes and data disk configurations</p>
<table>
	<tr>
		<th>VM Role</th>
		<th>VM Size</th>
		<th>Data Disks</th>
	</tr>
	<tr>
		<td>App - NetWeaver Gateway</td>
		<td>E4s_v3</td>
		<td>1xP4 (32GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - SAP PO</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP20 (512GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - Gateway FES</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP20 (512GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - SAP BW</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP20 (512GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - S/4HANA Utilities</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP6 (64GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - Convergent Charging</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - Convergent Invoicing</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP6 (64GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - SOM (CRM ABAP)</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP20 (512GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - SOM (CRM JAVA)</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP6 (64GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>App - Cloud Connector</td>
		<td>E4s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>DB - NetWeaver Gateway</td>
		<td>E8s_v3</td>
		<td>1xP4 (32GB), 1xP10 (128GB), 1xP6 (64GB), 1xP4 (32GB), 1xP6 (64GB), 1xP4 (32GB)</td>
	</tr>
	<tr>
		<td>DB - SAP PO</td>
		<td>E8s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>DB - Gateway FES</td>
		<td>E8s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>DB - SAP BW</td>
		<td>E8s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>DB - S/4HANA Utilities</td>
		<td>E8s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
	<tr>
		<td>DB - S/4HANA Hybris Billing</td>
		<td>E16s_v3</td>
		<td>1xP6 (64GB), 1xP10 (128GB), 1xP4 (32GB), 1xP6 (64GB)</td>
	</tr>
</table>
