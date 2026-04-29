---
description: A security rule within a Cloud NGFW rule stack.
layout: schema
name: SecurityRule
properties_list:
- description: Rule evaluation priority (lower numbers evaluated first).
  name: Priority
  type: integer
- description: ''
  name: RuleEntry
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-security-rule-schema.json
slug: cloud-ngfw-api-security-rule
source_filename: cloud-ngfw-api-security-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRule\",\n  \"description\": \"A security rule within a Cloud NGFW rule stack.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-security-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Rule evaluation priority (lower numbers evaluated first).\"\n    },\n    \"RuleEntry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"RuleName\": {\n          \"type\": \"string\"\n        },\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"Enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true\n        },\n        \"Source\": {\n          \"type\": \"object\",\n          \"description\": \"Traffic source matching criteria for a security rule.\",\n         \
  \ \"properties\": {\n            \"Cidrs\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Source CIDR blocks (e.g., 10.0.0.0/8).\"\n            },\n            \"Countries\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Source country codes (ISO 3166-1 alpha-2).\"\n            },\n            \"Feeds\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Threat intelligence feed names.\"\n            },\n            \"PrefixLists\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Names of prefix lists defined in the rule stack.\"\n            }\n          }\n \
  \       },\n        \"NegateSource\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"Destination\": {\n          \"type\": \"object\",\n          \"description\": \"Traffic destination matching criteria for a security rule.\",\n          \"properties\": {\n            \"Cidrs\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Destination CIDR blocks.\"\n            },\n            \"Countries\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Destination country codes.\"\n            },\n            \"Feeds\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"FqdnLists\": {\n              \"type\": \"array\",\n              \"items\"\
  : {\n                \"type\": \"string\"\n              },\n              \"description\": \"Names of FQDN lists defined in the rule stack.\"\n            },\n            \"PrefixLists\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"NegateDestination\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"Applications\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Application names to match (use any for all applications).\"\n        },\n        \"Category\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"URLCategoryNames\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"Feeds\": {\n              \"type\"\
  : \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"Protocol\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"APPLICATION-DEFAULT\",\n            \"TCP\",\n            \"UDP\",\n            \"ICMP\",\n            \"ANY\"\n          ]\n        },\n        \"Action\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Allow\",\n            \"DenyResetBoth\",\n            \"DenyResetServer\",\n            \"DenySilent\"\n          ]\n        },\n        \"DecryptionRuleType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SSLOutboundInspection\",\n            \"None\"\n          ]\n        },\n        \"AuditComment\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-security-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SecurityRule
---
