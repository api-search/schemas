---
description: SecurityRuleRequest schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: SecurityRuleRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: from
  type: array
- description: ''
  name: to
  type: array
- description: ''
  name: source
  type: array
- description: ''
  name: destination
  type: array
- description: ''
  name: source_user
  type: array
- description: ''
  name: application
  type: array
- description: ''
  name: service
  type: array
- description: ''
  name: category
  type: array
- description: ''
  name: action
  type: string
- description: ''
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
schema_file: json-schema/strata-cloud-manager-api-security-rule-request-schema.json
slug: strata-cloud-manager-api-security-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRuleRequest\",\n  \"description\": \"SecurityRuleRequest schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-security-rule-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"from\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"default\": [\n        \"any\"\n      ]\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"default\": [\n        \"any\"\n      ]\n    },\n    \"source\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"default\": [\n        \"any\"\n      ]\n    },\n    \"destination\": {\n\
  \      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"default\": [\n        \"any\"\n      ]\n    },\n    \"source_user\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"application\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"default\": [\n        \"any\"\n      ]\n    },\n    \"service\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"default\": [\n        \"application-default\"\n      ]\n    },\n    \"category\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"deny\",\n        \"drop\",\n        \"reset-client\",\n        \"reset-server\",\n        \"reset-both\"\n      ]\n    },\n    \"log_setting\": {\n      \"type\": \"string\"\n\
  \    },\n    \"profile_setting\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"group\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"action\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-security-rule-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SecurityRuleRequest
---
