---
description: SecurityRuleList schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: SecurityRuleList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: offset
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-security-rule-list-schema.json
slug: strata-cloud-manager-api-security-rule-list
source_filename: strata-cloud-manager-api-security-rule-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRuleList\",\n  \"description\": \"SecurityRuleList schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-security-rule-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A security policy rule defining traffic matching criteria and enforcement action applied by managed firewalls.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\",\n            \"readOnly\": true\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"folder\": {\n            \"type\": \"string\",\n            \"readOnly\": true\n    \
  \      },\n          \"position\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"pre\",\n              \"post\"\n            ]\n          },\n          \"from\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Source security zones.\"\n          },\n          \"to\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Destination security zones.\"\n          },\n          \"source\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Source addresses or address groups (use \\\"any\\\" for all).\"\n          },\n          \"destination\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\"\
  : \"Destination addresses or address groups.\"\n          },\n          \"source_user\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Source users or user groups.\"\n          },\n          \"application\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Applications to match (e.g., ssl, web-browsing).\"\n          },\n          \"service\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Service objects or application-default.\"\n          },\n          \"category\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"URL categories to match.\"\n          },\n          \"action\": {\n            \"type\"\
  : \"string\",\n            \"enum\": [\n              \"allow\",\n              \"deny\",\n              \"drop\",\n              \"reset-client\",\n              \"reset-server\",\n              \"reset-both\"\n            ]\n          },\n          \"log_setting\": {\n            \"type\": \"string\",\n            \"description\": \"Log forwarding profile name.\"\n          },\n          \"profile_setting\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"group\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"disabled\": {\n            \"type\": \"boolean\",\n            \"default\": false\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"tag\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n          \
  \  }\n          }\n        }\n      }\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-security-rule-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SecurityRuleList
---
