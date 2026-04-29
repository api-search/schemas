---
description: Attribute-based filter.
layout: schema
name: attr_based_filter
properties_list:
- description: Attribute name
  name: attrName
  type: string
- description: Attribute value
  name: attrValue
  type: string
- description: Value you want to match.
  name: match
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-attr_based_filter-schema.json
slug: cloud-identity-engine-api-attr_based_filter
source_filename: cloud-identity-engine-api-attr_based_filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"attr_based_filter\",\n  \"description\": \"Attribute-based filter.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-attr_based_filter-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attrName\": {\n      \"description\": \"Attribute name\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"User Principal Name\",\n        \"Common-Name\",\n        \"Name\",\n        \"Distinguished Name\",\n        \"SAM Account Name\",\n        \"Unique Identifier\"\n      ],\n      \"example\": \"Distinguished Name\"\n    },\n    \"attrValue\": {\n      \"description\": \"Attribute value\",\n      \"type\": \"string\",\n      \"example\": \"CN=Jack,UID=Park,DC=example,DC=com\"\n    },\n    \"match\": {\n      \"description\": \"Value you want to match.\",\n      \"type\": \"string\",\n     \
  \ \"enum\": [\n        \"equal\",\n        \"textSearch\"\n      ],\n      \"example\": \"equal\"\n    }\n  },\n  \"required\": [\n    \"attrName\",\n    \"attrValue\",\n    \"match\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-attr_based_filter-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: attr_based_filter
---
