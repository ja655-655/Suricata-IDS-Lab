# PROJECTNAME

## Objective

The goal of this lab was to configure custom IDS signatures in Suricata to analyze packet captures, trigger real time alerts, and parse JSON formatted telemetry for threat hunting and network forensics.

### Skills Learned

- IDS Signature Development: Creatiing custom Suricata rules using specific headers, traffic directions, payload contents (content:"GET";), and Signature IDs (sid).
- Packet Capture Testing: Executing Suricata in log reading mode against static ".pcap" files to simulate live network monitoring and validate rule syntax.
- Log Triage & Quick Analysis: Inspecting fast.log for immediate, single-line alert summaries and rapid signature verification.
- SON Log Parsing & Telemetry Analysis: Utilizing command line JSON processors (jq) to filter, format, and extract key fields (IP addresses, protocols, timestamps, user agents) from eve.json.
- Network Flow Correlation: Tracking session lifecycles across multiple log events by filtering and pivoting on unique flow_id values.

### Tools Used


- Suricata (IDS/IPS Engine): Command line network threat detection engine used to evaluate traffic against custom signatures.
- jq (Command-Line JSON Processor): Applied to parse, slice, and print structured data from eve.json logs.
- Linux CLI Utilities (ls, cat, less): Used for directory inspection and plain text file viewing (fast.log, custom.rules).
- Packet Capture Files (.pcap): Static packet dumps utilized for testing and offline analysis.

## Steps

*Ref 1: Scenario*

<img width="610" height="778" alt="image" src="https://github.com/user-attachments/assets/2484c95a-4abd-4bf5-96cd-2ba877778c70" />


<img width="618" height="203" alt="image" src="https://github.com/user-attachments/assets/0f1f3a5f-4577-428e-89a2-5a2845263c8d" />


*Ref 2: Examine a Custom Rule in Suricata*

<img width="736" height="539" alt="image" src="https://github.com/user-attachments/assets/779d8a70-c404-42e9-82bc-7a43ddb4e097" />

*Ref 3: Trigger a Custom Rule in Suricata*

<img width="733" height="151" alt="image" src="https://github.com/user-attachments/assets/d223c589-40a9-4e75-988d-1920da341a24" />

<img width="734" height="561" alt="image" src="https://github.com/user-attachments/assets/79c11856-77b2-43ae-9abf-11885bbe4e44" />


*Ref 4: Examine eve,json Output*

<img width="733" height="512" alt="image" src="https://github.com/user-attachments/assets/c8a5c9b9-8578-4fc2-99f4-4ec4a95892e9" />

<img width="734" height="725" alt="image" src="https://github.com/user-attachments/assets/8afaa47e-3375-468b-b1c3-fd21055c43b7" />

