# Honeypot-VM-Attack-Map
Built a honeypot VM in Azure to capture failed login attempts, analyzed attacker data in Log Analytics using KQL, and created an interactive attack map showing the geographic data of threat actors

## Tools & Technologies
- Microsoft Azure (VM + VN + Log Analytics)
- Kusto Query Language (KQL)
- Azure Workbooks for visualization

## Key Steps
1. Deployed a public-facing VM in an isolated Azure VNet.
2. Captured SecurityEvent logs (Event ID 4625 – failed logins).
3. Queried and enriched attacker IP data with GeoIP info.
4. Created an Azure Workbook map showing geographic attack data.

## Results
- Logged and analyzed hundreds of brute-force attempts from global IPs.
- Built an interactive attack map highlighting top attacker regions.
- Demonstrated practical SOC and log analysis skills.

## Ethics & Safety
All data was collected in a controlled, isolated environment.  
Raw IP addresses were anonymized before publication.
