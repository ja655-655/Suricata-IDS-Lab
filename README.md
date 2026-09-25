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
drag & drop screenshots here or use imgur and reference them using imgsrc

Every screenshot should have some text explaining what the screenshot is about.

Example below.

*Ref 1: Network Diagram*
