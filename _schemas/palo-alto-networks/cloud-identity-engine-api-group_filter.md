---
description: Group-based filter.
layout: schema
name: group_filter
properties_list:
- description: ''
  name: type
  type: string
- description: Attribute-based filter.
  name: name
  type: object
- description: ''
  name: level
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-group_filter-schema.json
slug: cloud-identity-engine-api-group_filter
source_filename: cloud-identity-engine-api-group_filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"group_filter\",\n  \"description\": \"Group-based filter.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-group_filter-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"group\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"description\": \"Attribute-based filter.\",\n      \"required\": [\n        \"attrName\",\n        \"attrValue\",\n        \"match\"\n      ],\n      \"properties\": {\n        \"attrName\": {\n          \"description\": \"Attribute name\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"User Principal Name\",\n            \"Common-Name\",\n            \"Name\",\n            \"Distinguished Name\",\n            \"SAM Account Name\",\n            \"Unique\
  \ Identifier\"\n          ],\n          \"example\": \"Distinguished Name\"\n        },\n        \"attrValue\": {\n          \"description\": \"Attribute value\",\n          \"type\": \"string\",\n          \"example\": \"CN=Jack,UID=Park,DC=example,DC=com\"\n        },\n        \"match\": {\n          \"description\": \"Value you want to match.\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"equal\",\n            \"textSearch\"\n          ],\n          \"example\": \"equal\"\n        }\n      }\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"immediate\",\n        \"recursive\"\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"name\",\n    \"level\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-group_filter-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: group_filter
---
