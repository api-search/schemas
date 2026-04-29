---
description: A network interface associated with a host.
layout: schema
name: HostInterface
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: mac
  type: '[''string'', ''null'']'
- description: ''
  name: ip
  type: '[''string'', ''null'']'
- description: ''
  name: ip6
  type: '[''string'', ''null'']'
- description: ''
  name: type
  type: string
- description: ''
  name: name
  type: '[''string'', ''null'']'
- description: ''
  name: subnet_id
  type: '[''integer'', ''null'']'
- description: ''
  name: subnet6_id
  type: '[''integer'', ''null'']'
- description: ''
  name: domain_id
  type: '[''integer'', ''null'']'
- description: Device identifier (e.g., eth0, ens192).
  name: identifier
  type: '[''string'', ''null'']'
- description: ''
  name: managed
  type: boolean
- description: ''
  name: primary
  type: boolean
- description: ''
  name: provision
  type: boolean
- description: ''
  name: virtual
  type: boolean
- description: VLAN tag.
  name: tag
  type: '[''string'', ''null'']'
- description: Maximum transmission unit.
  name: mtu
  type: '[''integer'', ''null'']'
- description: Parent interface identifier.
  name: attached_to
  type: '[''string'', ''null'']'
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-host-interface-schema.json
slug: red-hat-satellite-host-interface
source_filename: red-hat-satellite-host-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostInterface\",\n  \"type\": \"object\",\n  \"description\": \"A network interface associated with a host.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"mac\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"ip\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"ip6\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"subnet_id\": {\n      \"type\": \"['integer', 'null']\"\n    },\n    \"subnet6_id\": {\n      \"type\": \"['integer', 'null']\"\n    },\n    \"domain_id\": {\n      \"type\": \"['integer', 'null']\"\n    },\n    \"identifier\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Device identifier (e.g., eth0, ens192).\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\"\n    },\n\
  \    \"primary\": {\n      \"type\": \"boolean\"\n    },\n    \"provision\": {\n      \"type\": \"boolean\"\n    },\n    \"virtual\": {\n      \"type\": \"boolean\"\n    },\n    \"tag\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"VLAN tag.\"\n    },\n    \"mtu\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Maximum transmission unit.\"\n    },\n    \"attached_to\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Parent interface identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-host-interface-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: HostInterface
---
