---
description: A rule stack containing security policy for Cloud NGFW firewall instances.
layout: schema
name: RuleStack
properties_list:
- description: Unique name of the rule stack.
  name: RuleStackName
  type: string
- description: ''
  name: RuleStackEntry
  type: object
- description: Optimistic lock token for concurrent modification detection.
  name: UpdateToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-rule-stack-schema.json
slug: cloud-ngfw-api-rule-stack
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleStack\",\n  \"description\": \"A rule stack containing security policy for Cloud NGFW firewall instances.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-stack-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleStackName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the rule stack.\"\n    },\n    \"RuleStackEntry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"Scope\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Local\",\n            \"Global\"\n          ]\n        },\n        \"MinAppIdVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum App-ID content version required.\"\n        },\n        \"LookupXForwardedFor\"\
  : {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SecurityPolicy\",\n            \"None\"\n          ]\n        },\n        \"Profile\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"AntiSpywareProfile\": {\n              \"type\": \"string\"\n            },\n            \"AntiVirusProfile\": {\n              \"type\": \"string\"\n            },\n            \"VulnerabilityProfile\": {\n              \"type\": \"string\"\n            },\n            \"URLFilteringProfile\": {\n              \"type\": \"string\"\n            },\n            \"FileBlockingProfile\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"UpdateToken\": {\n      \"type\": \"string\",\n      \"description\": \"Optimistic lock token for concurrent modification detection.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-stack-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RuleStack
---
