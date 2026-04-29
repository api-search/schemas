---
description: GetIPSetResponse schema from Amazon GuardDuty API
layout: schema
name: GetIPSetResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Format
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-ip-set-response-schema.json
slug: guardduty-get-ip-set-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-ip-set-response-schema.json\",\n  \"title\": \"GetIPSetResponse\",\n  \"description\": \"GetIPSetResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The user-friendly name for the IPSet.\"\n        }\n      ]\n    },\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpSetFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"format\"\n          },\n          \"description\": \"The format of the file that contains the IPSet.\"\n        }\n      ]\n    },\n    \"Location\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Location\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"location\"\n          },\n          \"description\": \"The URI of the file that contains the IPSet.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpSetStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of IPSet file that was uploaded.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags of the IPSet resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Format\",\n    \"Location\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-ip-set-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetIPSetResponse
---
