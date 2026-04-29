---
description: CIScan schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: CIScan
properties_list:
- description: ''
  name: entityInfo
  type: object
- description: Whether the scan passed the configured policy thresholds.
  name: pass
  type: boolean
- description: ''
  name: vulnerabilitiesCount
  type: integer
- description: ''
  name: complianceIssuesCount
  type: integer
- description: ''
  name: vulnerabilityDistribution
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-ci-scan-schema.json
slug: prisma-cloud-compute-api-ci-scan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CIScan\",\n  \"description\": \"CIScan schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-ci-scan-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"_id\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ciImage\",\n            \"ciServerless\",\n            \"ciIaC\"\n          ]\n        },\n        \"hostname\": {\n          \"type\": \"string\"\n        },\n        \"scanTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"pass\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the scan\
  \ passed the configured policy thresholds.\"\n    },\n    \"vulnerabilitiesCount\": {\n      \"type\": \"integer\"\n    },\n    \"complianceIssuesCount\": {\n      \"type\": \"integer\"\n    },\n    \"vulnerabilityDistribution\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"critical\": {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-ci-scan-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CIScan
---
