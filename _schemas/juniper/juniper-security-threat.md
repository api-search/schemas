---
description: Schema representing a security threat or indicator of compromise as detected by Juniper ATP Cloud and SRX security platforms. Covers malware verdicts, IP/URL/domain reputation, and threat intelligence indicators.
layout: schema
name: Juniper Security Threat
properties_list:
- description: Unique identifier for the threat
  name: id
  type: string
- description: Type of threat indicator
  name: indicator_type
  type: string
- description: The actual indicator value (IP address, domain, URL, hash, etc.)
  name: indicator_value
  type: string
- description: Threat severity score from 0 (clean) to 10 (critical)
  name: threat_score
  type: integer
- description: Analysis verdict
  name: verdict
  type: string
- description: Confidence level of the assessment (0 to 1)
  name: confidence
  type: number
- description: Malware classification details (for file-based threats)
  name: malware_info
  type: object
- description: File details for file-based threats
  name: file_details
  type: object
- description: Threat categories (e.g., command-and-control, phishing, malware-distribution)
  name: categories
  type: array
- description: Intelligence sources that identified the threat
  name: sources
  type: array
- description: Devices that detected or were affected by this threat
  name: affected_devices
  type: array
- description: When the threat was first observed
  name: first_seen
  type: string
- description: When the threat was last observed
  name: last_seen
  type: string
- description: ''
  name: tags
  type: array
provider_name: Juniper Networks
provider_slug: juniper
schema_file: json-schema/juniper-security-threat.json
slug: juniper-security-threat
source_filename: juniper-security-threat.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/juniper/json-schema/juniper-security-threat.json\",\n  \"title\": \"Juniper Security Threat\",\n  \"description\": \"Schema representing a security threat or indicator of compromise as detected by Juniper ATP Cloud and SRX security platforms. Covers malware verdicts, IP/URL/domain reputation, and threat intelligence indicators.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the threat\"\n    },\n    \"indicator_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ip\",\n        \"domain\",\n        \"url\",\n        \"file_hash\",\n        \"email\",\n        \"certificate\"\n      ],\n      \"description\": \"Type of threat indicator\"\n    },\n    \"indicator_value\": {\n      \"type\": \"string\",\n      \"description\": \"The actual indicator value (IP\
  \ address, domain, URL, hash, etc.)\"\n    },\n    \"threat_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n      \"description\": \"Threat severity score from 0 (clean) to 10 (critical)\"\n    },\n    \"verdict\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"clean\",\n        \"suspicious\",\n        \"malicious\",\n        \"unknown\"\n      ],\n      \"description\": \"Analysis verdict\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Confidence level of the assessment (0 to 1)\"\n    },\n    \"malware_info\": {\n      \"type\": \"object\",\n      \"description\": \"Malware classification details (for file-based threats)\",\n      \"properties\": {\n        \"family\": {\n          \"type\": \"string\",\n          \"description\": \"Malware family name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n\
  \            \"trojan\",\n            \"ransomware\",\n            \"worm\",\n            \"adware\",\n            \"spyware\",\n            \"backdoor\",\n            \"rootkit\",\n            \"cryptominer\",\n            \"downloader\",\n            \"exploit\",\n            \"other\"\n          ]\n        },\n        \"variant\": {\n          \"type\": \"string\",\n          \"description\": \"Specific malware variant\"\n        }\n      }\n    },\n    \"file_details\": {\n      \"type\": \"object\",\n      \"description\": \"File details for file-based threats\",\n      \"properties\": {\n        \"sha256\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{64}$\"\n        },\n        \"sha1\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{40}$\"\n        },\n        \"md5\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{32}$\"\n        },\n        \"file_name\": {\n          \"type\": \"string\"\n   \
  \     },\n        \"file_type\": {\n          \"type\": \"string\"\n        },\n        \"file_size\": {\n          \"type\": \"integer\",\n          \"description\": \"File size in bytes\"\n        }\n      }\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Threat categories (e.g., command-and-control, phishing, malware-distribution)\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"Intelligence sources that identified the threat\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"feed_id\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"affected_devices\": {\n      \"type\": \"array\",\n      \"description\": \"Devices that detected or were affected by this threat\",\n      \"items\": {\n        \"type\": \"\
  object\",\n        \"properties\": {\n          \"device_id\": {\n            \"type\": \"string\"\n          },\n          \"hostname\": {\n            \"type\": \"string\"\n          },\n          \"action_taken\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"blocked\",\n              \"allowed\",\n              \"quarantined\",\n              \"logged\"\n            ]\n          }\n        }\n      }\n    },\n    \"first_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the threat was first observed\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the threat was last observed\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"indicator_type\", \"indicator_value\", \"verdict\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/json-schema/juniper-security-threat.json
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
title: Juniper Security Threat
---
