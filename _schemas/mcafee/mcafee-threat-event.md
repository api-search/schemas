---
description: A threat event represents a security detection from a McAfee product, including malware detections, intrusion attempts, policy violations, and behavioral anomalies reported by endpoints or network sensors.
layout: schema
name: McAfee Threat Event
properties_list:
- description: Auto-incremented unique event identifier
  name: id
  type: integer
- description: Name of the detected threat (e.g., W32/Conficker.worm, Generic.dx)
  name: threatName
  type: string
- description: Classification type of the threat
  name: threatType
  type: string
- description: Severity level of the threat (1=informational, 5=critical)
  name: threatSeverity
  type: integer
- description: Remediation action taken on the threat
  name: threatActionTaken
  type: string
- description: ISO 8601 timestamp when the threat was detected
  name: detectedAt
  type: string
- description: ISO 8601 timestamp when the event was received by the management server
  name: receivedAt
  type: string
- description: Hostname of the system where the threat was detected
  name: sourceHostName
  type: string
- description: IPv4 address of the source system
  name: sourceIPv4
  type: string
- description: IPv6 address of the source system
  name: sourceIPv6
  type: string
- description: MAC address of the source system
  name: sourceMac
  type: string
- description: Full file path of the affected file
  name: targetFileName
  type: string
- description: ''
  name: targetFileHash
  type: object
- description: Name of the McAfee product that detected the threat (e.g., VirusScan Enterprise, Endpoint Security)
  name: analyzerName
  type: string
- description: Version of the detecting product
  name: analyzerVersion
  type: string
- description: DAT (virus definition) version used during detection
  name: analyzerDATVersion
  type: string
- description: Scan engine version used during detection
  name: analyzerEngineVersion
  type: string
- description: Name of the user logged in at the time of detection
  name: userName
  type: string
- description: Name of the process associated with the threat
  name: processName
  type: string
- description: Hostname of the destination (for network-based threats)
  name: destinationHostName
  type: string
- description: IPv4 address of the destination
  name: destinationIPv4
  type: string
- description: Destination port (for network-based threats)
  name: destinationPort
  type: integer
- description: System Tree group path of the affected system in ePO
  name: epoGroupPath
  type: string
- description: McAfee Agent GUID of the reporting system
  name: agentGuid
  type: string
provider_name: McAfee (Trellix)
provider_slug: mcafee
schema_file: json-schema/mcafee-threat-event-schema.json
slug: mcafee-threat-event
source_filename: mcafee-threat-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.mcafee.com/schemas/mcafee/threat-event.json\",\n  \"title\": \"McAfee Threat Event\",\n  \"description\": \"A threat event represents a security detection from a McAfee product, including malware detections, intrusion attempts, policy violations, and behavioral anomalies reported by endpoints or network sensors.\",\n  \"type\": \"object\",\n  \"required\": [\"threatName\", \"detectedAt\", \"sourceHostName\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Auto-incremented unique event identifier\"\n    },\n    \"threatName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the detected threat (e.g., W32/Conficker.worm, Generic.dx)\",\n      \"minLength\": 1\n    },\n    \"threatType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"virus\",\n        \"trojan\",\n        \"worm\",\n        \"ransomware\",\n\
  \        \"rootkit\",\n        \"exploit\",\n        \"pup\",\n        \"adware\",\n        \"spyware\",\n        \"backdoor\",\n        \"fileless\",\n        \"unknown\"\n      ],\n      \"description\": \"Classification type of the threat\"\n    },\n    \"threatSeverity\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"description\": \"Severity level of the threat (1=informational, 5=critical)\"\n    },\n    \"threatActionTaken\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"cleaned\",\n        \"deleted\",\n        \"quarantined\",\n        \"blocked\",\n        \"allowed\",\n        \"denied\",\n        \"logged\",\n        \"none\"\n      ],\n      \"description\": \"Remediation action taken on the threat\"\n    },\n    \"detectedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the threat was detected\"\n    },\n    \"receivedAt\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event was received by the management server\"\n    },\n    \"sourceHostName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the system where the threat was detected\"\n    },\n    \"sourceIPv4\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IPv4 address of the source system\"\n    },\n    \"sourceIPv6\": {\n      \"type\": \"string\",\n      \"format\": \"ipv6\",\n      \"description\": \"IPv6 address of the source system\"\n    },\n    \"sourceMac\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\",\n      \"description\": \"MAC address of the source system\"\n    },\n    \"targetFileName\": {\n      \"type\": \"string\",\n      \"description\": \"Full file path of the affected file\"\n    },\n    \"targetFileHash\": {\n      \"$ref\": \"#/$defs/FileHash\"\n    },\n    \"analyzerName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the McAfee product that detected the threat (e.g., VirusScan Enterprise, Endpoint Security)\"\n    },\n    \"analyzerVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the detecting product\"\n    },\n    \"analyzerDATVersion\": {\n      \"type\": \"string\",\n      \"description\": \"DAT (virus definition) version used during detection\"\n    },\n    \"analyzerEngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Scan engine version used during detection\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the user logged in at the time of detection\"\n    },\n    \"processName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the process associated with the threat\"\n    },\n    \"destinationHostName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the destination (for network-based threats)\"\
  \n    },\n    \"destinationIPv4\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IPv4 address of the destination\"\n    },\n    \"destinationPort\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 65535,\n      \"description\": \"Destination port (for network-based threats)\"\n    },\n    \"epoGroupPath\": {\n      \"type\": \"string\",\n      \"description\": \"System Tree group path of the affected system in ePO\"\n    },\n    \"agentGuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"McAfee Agent GUID of the reporting system\"\n    }\n  },\n  \"$defs\": {\n    \"FileHash\": {\n      \"type\": \"object\",\n      \"description\": \"Cryptographic hash values for a file\",\n      \"properties\": {\n        \"md5\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{32}$\",\n          \"description\": \"MD5 hash of the file\"\n        },\n        \"sha1\": {\n\
  \          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{40}$\",\n          \"description\": \"SHA-1 hash of the file\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{64}$\",\n          \"description\": \"SHA-256 hash of the file\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/json-schema/mcafee-threat-event-schema.json
tags:
- Antivirus
- Cybersecurity
- Endpoint Protection
- Security
- Threat Intelligence
title: McAfee Threat Event
---
