---
description: FindingDetails schema
layout: schema
name: FindingDetails
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-finding-details-schema.json
slug: inspector-finding-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-details-schema.json\",\n  \"title\": \"FindingDetails\",\n  \"description\": \"FindingDetails schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"cisaData\": {\n        \"$ref\": \"#/components/schemas/CisaData\"\n      },\n      \"cwes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Cwes\"\n          },\n          {\n            \"description\": \"The Common Weakness Enumerations (CWEs) associated with the vulnerability.\"\n          }\n        ]\n      },\n      \"epssScore\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Double\"\n          },\n          {\n            \"description\": \"The Exploit Prediction Scoring System (EPSS) score of the vulnerability.\"\
  \n          }\n        ]\n      },\n      \"evidences\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EvidenceList\"\n          },\n          {\n            \"description\": \"Information on the evidence of the vulnerability.\"\n          }\n        ]\n      },\n      \"exploitObserved\": {\n        \"$ref\": \"#/components/schemas/ExploitObserved\"\n      },\n      \"findingArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FindingArn\"\n          },\n          {\n            \"description\": \"The finding ARN that the vulnerability details are associated with.\"\n          }\n        ]\n      },\n      \"referenceUrls\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VulnerabilityReferenceUrls\"\n          },\n          {\n            \"description\": \"The reference URLs for the vulnerability data.\"\n          }\n        ]\n      },\n      \"riskScore\": {\n        \"allOf\"\
  : [\n          {\n            \"$ref\": \"#/components/schemas/RiskScore\"\n          },\n          {\n            \"description\": \"The risk score of the vulnerability.\"\n          }\n        ]\n      },\n      \"tools\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Tools\"\n          },\n          {\n            \"description\": \"The known malware tools or kits that can exploit the vulnerability.\"\n          }\n        ]\n      },\n      \"ttps\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Ttps\"\n          },\n          {\n            \"description\": \"The MITRE adversary tactics, techniques, or procedures (TTPs) associated with the vulnerability.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Details of the vulnerability identified in a finding.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-details-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FindingDetails
---
