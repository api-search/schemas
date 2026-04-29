---
description: A NAT policy rule defining source or destination address translation for matching traffic flows.
layout: schema
name: NatRule
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
- description: Source zones.
  name: from
  type: array
- description: Destination zones.
  name: to
  type: array
- description: ''
  name: source
  type: array
- description: ''
  name: destination
  type: array
- description: Service object name or any.
  name: service
  type: string
- description: ''
  name: source_translation
  type: object
- description: ''
  name: destination_translation
  type: object
- description: ''
  name: nat_type
  type: string
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
schema_file: json-schema/strata-cloud-manager-api-nat-rule-schema.json
slug: strata-cloud-manager-api-nat-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NatRule\",\n  \"description\": \"A NAT policy rule defining source or destination address translation for matching traffic flows.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-nat-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pre\",\n        \"post\"\n      ]\n    },\n    \"from\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Source zones.\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n  \
  \    \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Destination zones.\"\n    },\n    \"source\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"destination\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"Service object name or any.\"\n    },\n    \"source_translation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dynamic_ip_and_port\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"translated_address\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"static_ip\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"translated_address\": {\n              \"type\": \"string\"\
  \n            },\n            \"bi_directional\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"destination_translation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"translated_address\": {\n          \"type\": \"string\"\n        },\n        \"translated_port\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"nat_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ipv4\",\n        \"nat64\",\n        \"nptv6\"\n      ]\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-nat-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NatRule
---
