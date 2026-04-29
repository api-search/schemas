---
description: Schema for a forwarded PAN-OS WildFire submission log entry. WildFire logs record the results of file analysis by the WildFire cloud-based sandbox malware analysis service, providing verdicts and analysis report links for detected threats.
layout: schema
name: WildfireLogPayload
properties_list:
- description: Timestamp when the WildFire log entry was received by Strata Logging Service.
  name: receive_time
  type: string
- description: Serial number of the Palo Alto Networks device that submitted the file to WildFire and generated this log entry.
  name: serial
  type: string
- description: Log type identifier, always WILDFIRE for WildFire log entries.
  name: type
  type: string
- description: Source IP address of the session from which the file was captured.
  name: src
  type: string
- description: Destination IP address of the session from which the file was captured.
  name: dst
  type: string
- description: Application identified by App-ID in the session from which the file was captured.
  name: app
  type: string
- description: Name of the file that was submitted to WildFire for analysis.
  name: filename
  type: string
- description: File type of the submitted file (e.g., PE, PDF, APK, Adobe Flash, Microsoft Office, script, Java Applet).
  name: filetype
  type: string
- description: SHA-256 cryptographic hash of the submitted file, used as the unique file identifier in the WildFire cloud database.
  name: file_hash
  type: string
- description: Size of the submitted file in bytes.
  name: file_size
  type: integer
- description: WildFire analysis verdict for the submitted file indicating whether it is benign, malicious malware, potentially unwanted grayware, a phishing document, or pending analysis completion.
  name: verdict
  type: string
- description: Action applied to the file by the WildFire security profile based on the analysis verdict.
  name: action
  type: string
- description: URL to the full WildFire analysis report in the Palo Alto Networks WildFire portal, providing detailed behavioral analysis results.
  name: report_url
  type: string
- description: Source user identity if User-ID is enabled.
  name: src_user
  type: string
- description: Name of the security policy rule under which the file was captured and submitted to WildFire.
  name: rule_name
  type: string
- description: Hostname of the firewall that captured the file and generated this WildFire log entry.
  name: device_name
  type: string
- description: Virtual system name or identifier on the firewall.
  name: vsys
  type: string
- description: Name of the log forwarding profile that forwarded this log entry.
  name: log_forwarding_profile
  type: string
- description: Output format in which this log entry was forwarded.
  name: output_format
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-forwarding-wildfire-log-payload-schema.json
slug: strata-logging-forwarding-wildfire-log-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WildfireLogPayload\",\n  \"description\": \"Schema for a forwarded PAN-OS WildFire submission log entry. WildFire logs record the results of file analysis by the WildFire cloud-based sandbox malware analysis service, providing verdicts and analysis report links for detected threats.\\n\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-forwarding-wildfire-log-payload-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"receive_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the WildFire log entry was received by Strata Logging Service.\\n\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the Palo Alto Networks device that submitted the file to WildFire and generated this log entry.\\n\"\
  \n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WILDFIRE\"\n      ],\n      \"description\": \"Log type identifier, always WILDFIRE for WildFire log entries.\\n\"\n    },\n    \"src\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the session from which the file was captured.\"\n    },\n    \"dst\": {\n      \"type\": \"string\",\n      \"description\": \"Destination IP address of the session from which the file was captured.\\n\"\n    },\n    \"app\": {\n      \"type\": \"string\",\n      \"description\": \"Application identified by App-ID in the session from which the file was captured.\\n\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the file that was submitted to WildFire for analysis.\"\n    },\n    \"filetype\": {\n      \"type\": \"string\",\n      \"description\": \"File type of the submitted file (e.g., PE, PDF, APK, Adobe Flash, Microsoft Office, script, Java Applet).\\\
  n\"\n    },\n    \"file_hash\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 cryptographic hash of the submitted file, used as the unique file identifier in the WildFire cloud database.\\n\"\n    },\n    \"file_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the submitted file in bytes.\"\n    },\n    \"verdict\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"benign\",\n        \"malware\",\n        \"grayware\",\n        \"phishing\",\n        \"pending\"\n      ],\n      \"description\": \"WildFire analysis verdict for the submitted file indicating whether it is benign, malicious malware, potentially unwanted grayware, a phishing document, or pending analysis completion.\\n\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"block\"\n      ],\n      \"description\": \"Action applied to the file by the WildFire security profile based on the analysis verdict.\\n\"\n    },\n\
  \    \"report_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full WildFire analysis report in the Palo Alto Networks WildFire portal, providing detailed behavioral analysis results.\\n\"\n    },\n    \"src_user\": {\n      \"type\": \"string\",\n      \"description\": \"Source user identity if User-ID is enabled.\"\n    },\n    \"rule_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the security policy rule under which the file was captured and submitted to WildFire.\\n\"\n    },\n    \"device_name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the firewall that captured the file and generated this WildFire log entry.\\n\"\n    },\n    \"vsys\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual system name or identifier on the firewall.\"\n    },\n    \"log_forwarding_profile\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the log forwarding profile\
  \ that forwarded this log entry.\\n\"\n    },\n    \"output_format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CSV\",\n        \"LEEF\",\n        \"CEF\",\n        \"JSON\",\n        \"PARQUET\"\n      ],\n      \"description\": \"Output format in which this log entry was forwarded.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-forwarding-wildfire-log-payload-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: WildfireLogPayload
---
