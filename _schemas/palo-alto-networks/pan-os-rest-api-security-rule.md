---
description: A security policy rule controlling traffic flow between zones based on source, destination, application, service, and user criteria.
layout: schema
name: SecurityRule
properties_list:
- description: Unique name of the security rule.
  name: '@name'
  type: string
- description: ''
  name: from
  type: object
- description: ''
  name: to
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: source-user
  type: object
- description: ''
  name: application
  type: object
- description: ''
  name: service
  type: object
- description: ''
  name: category
  type: object
- description: Action to take on matching traffic.
  name: action
  type: string
- description: Log at session start.
  name: log-start
  type: string
- description: Log at session end.
  name: log-end
  type: string
- description: Log forwarding profile name.
  name: log-setting
  type: string
- description: Security profile group or individual profiles.
  name: profile-setting
  type: object
- description: Whether the rule is disabled.
  name: disabled
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-security-rule-schema.json
slug: pan-os-rest-api-security-rule
source_filename: pan-os-rest-api-security-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityRule\",\n  \"description\": \"A security policy rule controlling traffic flow between zones based on source, destination, application, service, and user criteria.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-security-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the security rule.\"\n    },\n    \"from\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Source zones (e.g., trust, untrust).\"\n        }\n      }\n    },\n    \"to\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\"\
  ,\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Destination zones.\"\n        }\n      }\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Source addresses or address groups (use \\\"any\\\" for all).\"\n        }\n      }\n    },\n    \"destination\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Destination addresses or address groups.\"\n        }\n      }\n    },\n    \"source-user\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"\
  description\": \"Source users or user groups (use \\\"any\\\" for all).\"\n        }\n      }\n    },\n    \"application\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Application names (e.g., ssl, web-browsing, any).\"\n        }\n      }\n    },\n    \"service\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Service objects or application-default to use application native ports.\"\n        }\n      }\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"URL categories.\"\n\
  \        }\n      }\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"deny\",\n        \"drop\",\n        \"reset-client\",\n        \"reset-server\",\n        \"reset-both\"\n      ],\n      \"description\": \"Action to take on matching traffic.\"\n    },\n    \"log-start\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"description\": \"Log at session start.\"\n    },\n    \"log-end\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"description\": \"Log at session end.\"\n    },\n    \"log-setting\": {\n      \"type\": \"string\",\n      \"description\": \"Log forwarding profile name.\"\n    },\n    \"profile-setting\": {\n      \"type\": \"object\",\n      \"description\": \"Security profile group or individual profiles.\",\n      \"properties\": {\n        \"group\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"member\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"disabled\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"description\": \"Whether the rule is disabled.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-security-rule-schema.json
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
