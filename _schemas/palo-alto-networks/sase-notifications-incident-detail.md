---
description: Detailed information about a SASE security incident for enrichment and correlation.
layout: schema
name: IncidentDetail
properties_list:
- description: Unique incident identifier.
  name: incidentId
  type: string
- description: Incident type classification.
  name: type
  type: string
- description: ''
  name: severity
  type: string
- description: Incident title.
  name: title
  type: string
- description: Incident description.
  name: description
  type: string
- description: Tenant Service Group identifier.
  name: tsg_id
  type: string
- description: Incident category.
  name: category
  type: string
- description: Source of the incident detection.
  name: detectionSource
  type: string
- description: ''
  name: timestamp
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-incident-detail-schema.json
slug: sase-notifications-incident-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentDetail\",\n  \"description\": \"Detailed information about a SASE security incident for enrichment and correlation.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-incident-detail-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incidentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique incident identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Incident type classification.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"informational\",\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Incident title.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Incident description.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group identifier.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Incident category.\"\n    },\n    \"detectionSource\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the incident detection.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-incident-detail-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IncidentDetail
---
