# Honeypot-VM-Attack-Map
This project captures and analyzes failed login attempts to a honeypot VM.
Using Azure Sentinel KQL queries and a GeoIP watchlist, failed authentication events were aggregated by region and visualized as a global attack heatmap.
Sensitive data has been sanitized prior to publication.

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
- ![Attack Map](https://raw.githubusercontent.com/joar7160-byte/Honeypot-VM-Attack-Map/main/Visualization/AttackMap/AttackMap.jpg)

## Ethics & Safety
All data was collected in a controlled, isolated environment.  
Raw IP addresses were anonymized before publication.
