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
2. Captured SecurityEvent logs (Event ID 4625 : failed logins).
- <img width="2035" height="935" alt="LogQuery1" src="https://github.com/user-attachments/assets/141489ac-539a-4d0b-bb43-9313d1df0312" />


3. Queried and enriched attacker IP data with GeoIP info.

- <img width="1611" height="780" alt="Log2" src="https://github.com/user-attachments/assets/66693b97-3654-4b5b-b978-5ab4c5d2b1bc" />
- <img width="1581" height="727" alt="Log3" src="https://github.com/user-attachments/assets/cb3eef7f-61aa-4775-9afc-d87fd6774ece" />
- <img width="1574" height="761" alt="log4" src="https://github.com/user-attachments/assets/54594857-e946-40be-8b44-a9c3ee4b16f0" />


4. Created an Azure Workbook map showing geographic attack data.
- <img width="1426" height="574" alt="image" src="https://github.com/user-attachments/assets/433cda8f-1266-4707-af48-6ca704305b5f" />

## Results
- Logged and analyzed hundreds of brute-force attempts from global IPs.
- Built an interactive attack map highlighting top attacker regions.
- Demonstrated practical SOC and log analysis skills.

