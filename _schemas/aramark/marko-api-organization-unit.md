---
description: OrganizationUnit schema from Aramark Marko API
layout: schema
name: OrganizationUnit
properties_list:
- description: Unique organization unit identifier
  name: id
  type: string
- description: Organization unit name
  name: name
  type: string
- description: Organization unit type
  name: type
  type: string
- description: Parent organization unit identifier
  name: parentId
  type: string
- description: Number of locations under this unit
  name: locationCount
  type: integer
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-organization-unit-schema.json
slug: marko-api-organization-unit
source_filename: marko-api-organization-unit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique organization unit identifier\",\n      \"example\": \"ORG-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization unit name\",\n      \"example\": \"Northeast District\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Organization unit type\",\n      \"enum\": [\n        \"REGION\",\n        \"DISTRICT\",\n        \"LOCATION\",\n        \"ACCOUNT\"\n      ],\n      \"example\": \"DISTRICT\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent organization unit identifier\",\n      \"example\": \"REGION-NE\"\n    },\n    \"locationCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of locations under this unit\",\n      \"example\": 45\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"\
  $id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-organization-unit-schema.json\",\n  \"title\": \"OrganizationUnit\",\n  \"description\": \"OrganizationUnit schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-organization-unit-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: OrganizationUnit
---
