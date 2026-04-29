---
description: A security policy rule defining traffic matching criteria and enforcement action applied by managed firewalls.
layout: schema
name: SecurityRule
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: folder
  type: string
- description: ''
  name: position
  type: string
- description: Source security zones.
  name: from
  type: array
- description: Destination security zones.
  name: to
  type: array
- description: Source addresses or address groups (use "any" for all).
  name: source
  type: array
- description: Destination addresses or address groups.
  name: destination
  type: array
- description: Source users or user groups.
  name: source_user
  type: array
- description: Applications to match (e.g., ssl, web-browsing).
  name: application
  type: array
- description: Service objects or application-default.
  name: service
  type: array
- description: URL categories to match.
  name: category
  type: array
- description: ''
  name: action
  type: string
- description: Log forwarding profile name.
  name: log_setting
  type: string
- description: ''
  name: profile_setting
  type: object
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-security-rule-schema.json
slug: strata-cloud-manager-api-security-rule
source_filename: strata-cloud-manager-api-security-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRule\",\n  \"description\": \"A security policy rule defining traffic matching criteria and enforcement action applied by managed firewalls.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-security-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pre\",\n        \"post\"\n      ]\n    },\n    \"from\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Source security zones.\"\n    },\n    \"to\": {\n\
  \      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Destination security zones.\"\n    },\n    \"source\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Source addresses or address groups (use \\\"any\\\" for all).\"\n    },\n    \"destination\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Destination addresses or address groups.\"\n    },\n    \"source_user\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Source users or user groups.\"\n    },\n    \"application\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Applications to match (e.g., ssl, web-browsing).\"\n    },\n    \"service\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"string\"\n      },\n      \"description\": \"Service objects or application-default.\"\n    },\n    \"category\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"URL categories to match.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"deny\",\n        \"drop\",\n        \"reset-client\",\n        \"reset-server\",\n        \"reset-both\"\n      ]\n    },\n    \"log_setting\": {\n      \"type\": \"string\",\n      \"description\": \"Log forwarding profile name.\"\n    },\n    \"profile_setting\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"group\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"\
  tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-security-rule-schema.json
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
