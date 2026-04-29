---
description: A QoS policy rule classifying traffic into QoS classes for bandwidth management and prioritization.
layout: schema
name: QosRule
properties_list:
- description: Unique name of the QoS rule.
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
  name: application
  type: object
- description: ''
  name: service
  type: object
- description: DSCP/TOS marking settings.
  name: dscp-tos
  type: object
- description: ''
  name: action
  type: object
- description: ''
  name: disabled
  type: string
- description: ''
  name: description
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-qos-rule-schema.json
slug: pan-os-rest-api-qos-rule
source_filename: pan-os-rest-api-qos-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QosRule\",\n  \"description\": \"A QoS policy rule classifying traffic into QoS classes for bandwidth management and prioritization.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-qos-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the QoS rule.\"\n    },\n    \"from\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Source zones.\"\n        }\n      }\n    },\n    \"to\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n    \
  \      },\n          \"description\": \"Destination zones.\"\n        }\n      }\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"destination\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"application\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"service\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n\
  \    },\n    \"dscp-tos\": {\n      \"type\": \"object\",\n      \"description\": \"DSCP/TOS marking settings.\",\n      \"properties\": {\n        \"any\": {\n          \"type\": \"object\"\n        }\n      }\n    },\n    \"action\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"class\": {\n          \"type\": \"string\",\n          \"description\": \"QoS class number (1-8).\"\n        }\n      }\n    },\n    \"disabled\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-qos-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: QosRule
---
