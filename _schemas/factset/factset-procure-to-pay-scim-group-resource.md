---
description: ''
layout: schema
name: GroupResource
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: externalId
  type: string
- description: A human-readable name for the Group.
  name: displayName
  type: string
- description: A description for the Group.
  name: description
  type: string
- description: A list of members of the Group.
  name: members
  type: array
- description: ''
  name: urn:scim:schemas:extension:FactSet:EnterpriseHosting:1.0:Group
  type: object
- description: ''
  name: urn:scim:schemas:extension:FactSet:VRS:1.0:Group
  type: object
- description: ''
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-group-resource-schema.json
slug: factset-procure-to-pay-scim-group-resource
source_filename: factset-procure-to-pay-scim-group-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the Group.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for the Group.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"A list of members of the Group.\"\n    },\n    \"urn:scim:schemas:extension:FactSet:EnterpriseHosting:1.0:Group\": {\n      \"type\": \"object\"\n    },\n    \"urn:scim:schemas:extension:FactSet:VRS:1.0:Group\": {\n      \"type\": \"object\"\n    },\n    \"meta\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-group-resource-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: GroupResource
---
