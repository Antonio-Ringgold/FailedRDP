<h1>Azure Sentinel Failed RDP Map</h1>


<h2>Description</h2>
<b>The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.
</b>
<br />
<br />
The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot.
We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to
look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

<img src="https://i.imgur.com/KOPz3LO.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from Russia coming in. Custom logs being output with geodata</h2>

<img src="https://i.imgur.com/p903U9q.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>The same custom logs but displayed in Azure with a quick script to organize the data output.</h2>

<img src="https://i.imgur.com/LNcKIfz.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>

<h2>World map of RDP attacks after 24 hours</h2>

<img src="https://i.imgur.com/q6mYNZO.png" height="100%" width="85%" alt="Image Analysis Dataflow"/>
</p>
