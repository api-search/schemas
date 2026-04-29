---
description: Contains files infected with the given threat providing details of malware name and severity.
layout: schema
name: ScanThreatName
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: ItemCount
  type: object
- description: ''
  name: FilePaths
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-threat-name-schema.json
slug: guardduty-scan-threat-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-threat-name-schema.json\",\n  \"title\": \"ScanThreatName\",\n  \"description\": \"Contains files infected with the given threat providing details of malware name and severity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the identified threat.\"\n        }\n      ]\n    },\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"severity\"\n          },\n          \"description\": \"Severity of threat identified as part of the malware scan.\"\
  \n        }\n      ]\n    },\n    \"ItemCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"itemCount\"\n          },\n          \"description\": \"Total number of files infected with given threat.\"\n        }\n      ]\n    },\n    \"FilePaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilePaths\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filePaths\"\n          },\n          \"description\": \"List of infected files in EBS volume with details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-threat-name-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanThreatName
---
