---
description: SecurityRule schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: SecurityRule
properties_list:
- description: ''
  name: id
  type: string
- description: Name of the security rule.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: disabled
  type: boolean
- description: Source security zones.
  name: from
  type: array
- description: Destination security zones.
  name: to
  type: array
- description: Source addresses or address groups.
  name: source
  type: array
- description: Destination addresses or address groups.
  name: destination
  type: array
- description: Source user or user group names.
  name: source_user
  type: array
- description: Applications to match.
  name: application
  type: array
- description: Services or service groups to match.
  name: service
  type: array
- description: URL categories to match.
  name: category
  type: array
- description: Action to take when the rule matches.
  name: action
  type: string
- description: ''
  name: profile_setting
  type: object
- description: Log forwarding profile name.
  name: log_setting
  type: string
- description: ''
  name: tag
  type: array
- description: ''
  name: folder
  type: string
- description: ''
  name: position
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-security-rule-schema.json
slug: prisma-access-api-security-rule
source_filename: prisma-access-api-security-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRule\",\n  \"description\": \"SecurityRule schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-security-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the security rule.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"from\": {\n      \"type\": \"array\",\n      \"description\": \"Source security zones.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"description\": \"Destination security\
  \ zones.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source\": {\n      \"type\": \"array\",\n      \"description\": \"Source addresses or address groups.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"destination\": {\n      \"type\": \"array\",\n      \"description\": \"Destination addresses or address groups.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source_user\": {\n      \"type\": \"array\",\n      \"description\": \"Source user or user group names.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"application\": {\n      \"type\": \"array\",\n      \"description\": \"Applications to match.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"service\": {\n      \"type\": \"array\",\n      \"description\": \"Services or service groups to match.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"category\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"URL categories to match.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"deny\",\n        \"drop\",\n        \"reset-client\",\n        \"reset-server\",\n        \"reset-both\"\n      ],\n      \"description\": \"Action to take when the rule matches.\"\n    },\n    \"profile_setting\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"group\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Security profile group names.\"\n        }\n      }\n    },\n    \"log_setting\": {\n      \"type\": \"string\",\n      \"description\": \"Log forwarding profile name.\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"folder\": {\n      \"type\": \"\
  string\",\n      \"readOnly\": true\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pre\",\n        \"post\"\n      ],\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"from\",\n    \"to\",\n    \"source\",\n    \"destination\",\n    \"application\",\n    \"action\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-security-rule-schema.json
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
