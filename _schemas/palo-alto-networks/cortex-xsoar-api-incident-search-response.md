---
description: IncidentSearchResponse schema from Palo Alto Networks Cortex XSOAR REST API
layout: schema
name: IncidentSearchResponse
properties_list:
- description: ''
  name: total
  type: object
- description: ''
  name: incidents
  type: array
- description: ''
  name: searchResultTotal
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-incident-search-response-schema.json
slug: cortex-xsoar-api-incident-search-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentSearchResponse\",\n  \"description\": \"IncidentSearchResponse schema from Palo Alto Networks Cortex XSOAR REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-incident-search-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"integer\"\n        },\n        \"relation\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"incidents\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A Cortex XSOAR incident representing a security event under investigation.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique incident identifier.\"\
  ,\n            \"readOnly\": true\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Incident name or title.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Incident type (maps to an incident type definition).\"\n          },\n          \"status\": {\n            \"type\": \"integer\",\n            \"description\": \"Incident status code: 0 (Pending), 1 (Active), 2 (Done), 3 (Archive).\",\n            \"enum\": [\n              0,\n              1,\n              2,\n              3\n            ]\n          },\n          \"severity\": {\n            \"type\": \"integer\",\n            \"description\": \"Severity level: 0 (Unknown), 1 (Informational), 2 (Low), 3 (Medium), 4 (High), 5 (Critical).\",\n            \"enum\": [\n              0,\n              1,\n              2,\n              3,\n              4,\n              5\n            ]\n          },\n          \"owner\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"Username of the analyst assigned to this incident.\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Incident creation timestamp.\",\n            \"readOnly\": true\n          },\n          \"modified\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Last modification timestamp.\",\n            \"readOnly\": true\n          },\n          \"occurred\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp when the security event occurred.\"\n          },\n          \"closed\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Incident closure timestamp.\"\n          },\n          \"closeReason\": {\n            \"type\": \"string\",\n  \
  \          \"description\": \"Reason for closing the incident.\"\n          },\n          \"closeNotes\": {\n            \"type\": \"string\",\n            \"description\": \"Notes added when closing the incident.\"\n          },\n          \"labels\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\"\n                },\n                \"value\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"description\": \"Key-value label pairs attached to the incident.\"\n          },\n          \"details\": {\n            \"type\": \"string\",\n            \"description\": \"Incident details or description.\"\n          },\n          \"investigationId\": {\n            \"type\": \"string\",\n            \"description\": \"Associated investigation ID.\",\n            \"readOnly\": true\n\
  \          },\n          \"playbookId\": {\n            \"type\": \"string\",\n            \"description\": \"Playbook assigned to this incident.\"\n          },\n          \"sourceInstance\": {\n            \"type\": \"string\",\n            \"description\": \"Integration instance that created this incident.\"\n          },\n          \"sourceBrand\": {\n            \"type\": \"string\",\n            \"description\": \"Integration brand that created this incident.\"\n          },\n          \"rawJson\": {\n            \"type\": \"string\",\n            \"description\": \"Raw JSON payload from the originating event.\"\n          },\n          \"CustomFields\": {\n            \"type\": \"object\",\n            \"description\": \"Custom field values specific to the incident type.\",\n            \"additionalProperties\": true\n          }\n        }\n      }\n    },\n    \"searchResultTotal\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-incident-search-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IncidentSearchResponse
---
