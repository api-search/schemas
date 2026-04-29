---
description: A configured instance of an integration in Cortex XSOAR.
layout: schema
name: IntegrationInstance
properties_list:
- description: ''
  name: id
  type: string
- description: Unique name of this instance.
  name: name
  type: string
- description: Integration brand name.
  name: brand
  type: string
- description: ''
  name: enabled
  type: string
- description: ''
  name: isIntegrationScript
  type: boolean
- description: ''
  name: incomingMapperId
  type: string
- description: ''
  name: mappingId
  type: string
- description: Integration configuration parameters.
  name: configuration
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-integration-instance-schema.json
slug: cortex-xsoar-api-integration-instance
source_filename: cortex-xsoar-api-integration-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntegrationInstance\",\n  \"description\": \"A configured instance of an integration in Cortex XSOAR.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-integration-instance-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of this instance.\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Integration brand name.\"\n    },\n    \"enabled\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"true\",\n        \"false\"\n      ]\n    },\n    \"isIntegrationScript\": {\n      \"type\": \"boolean\"\n    },\n    \"incomingMapperId\": {\n      \"type\": \"string\"\n    },\n    \"mappingId\": {\n      \"type\": \"string\"\n    },\n   \
  \ \"configuration\": {\n      \"type\": \"object\",\n      \"description\": \"Integration configuration parameters.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-integration-instance-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IntegrationInstance
---
