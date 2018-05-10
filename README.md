<h1>Azure SAP HANA Deployment Template</h1>
<p>This template takes a minimum amount of parameters and deploys one or more VMs, customized for use with 3-tier SAP HANA, using a variety of custom and gallery operating system images. Each VM is configured with two NICs, each with one Static IP Addresses.</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FARMTest%2Fmaster%2Fazuredeploy.single.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploly SINGLE SAP VM</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FARMTest%2Fmaster%2Fazuredeploy.full.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a FULL SAP Environment (10 VMs - ISU, CRM, PIC, BWA, JVA, NGW, MOB, EWM, CEV, PIN)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FARMTest%2Fmaster%2Fazuredeploy.functional.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a FUNCTIONAL SAP Environment (7 VMs - ISU, CRM, PIC, JVA, NGW, MOB, EWM)</p>
<p><a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsimonhutson%2FARMTest%2Fmaster%2Fazuredeploy.core.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png" />
</a>
Deploy a CORE SAP Environment (5 VMs - ISU, CRM, PIC, JVA, NGW)</p>
<p>The VMs are configured using the following sizes, and data disk configurations</p>
<table>
	<tr>
		<th>VM Role</th>
		<th>VM Size</th>
		<th>Data Disks</th>
	</tr>
	<tr>
		<td>ISU</td>
		<td>E4s_v3</td>
		<td>1xP6 1xP30 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>CRM</td>
		<td>E4s_v3</td>
		<td>1xP6 1xP20 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>PIC</td>
		<td>D4s_v3</td>
		<td>1xP6 1xP20 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>BWA</td>
		<td>D4s_v3</td>
		<td>1xP6 1xP20 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>MOB</td>
		<td>E2s_v3</td>
		<td>1xP6 1xP6 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>EWM</td>
		<td>E2s_v3</td>
		<td>1xP6 1xP10 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>JVA</td>
		<td>E2s_v3</td>
		<td>1xP6 1xP6 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>CEV</td>
		<td>E2s_v3</td>
		<td>1xP6 1xP20 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>PIN</td>
		<td>E2s_v3</td>
		<td>1xP6 1xP6 1xP4 1xP6</td>
	</tr>
	<tr>
		<td>NGW</td>
		<td>E2s_v3</td>
		<td>1xP6 1xP10 1xP4 1xP6</td>
	</tr>
</table>
