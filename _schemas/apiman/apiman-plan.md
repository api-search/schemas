---
description: Schema representing an API plan in Apiman with associated policies
layout: schema
name: Apiman Plan
properties_list:
- description: Organization identifier owning this plan
  name: organizationId
  type: string
- description: Unique identifier for the plan
  name: id
  type: string
- description: Name of the plan
  name: name
  type: string
- description: Description of the plan
  name: description
  type: string
- description: Username of the user who created the plan
  name: createdBy
  type: string
- description: Timestamp when the plan was created
  name: createdOn
  type: string
- description: Policies applied to this plan
  name: policies
  type: array
provider_name: Apiman
provider_slug: apiman
schema_file: json-schema/apiman-plan-schema.json
slug: apiman-plan
source_filename: apiman-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apiman/main/json-schema/apiman-plan-schema.json\",\n  \"title\": \"Apiman Plan\",\n  \"description\": \"Schema representing an API plan in Apiman with associated policies\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization identifier owning this plan\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the plan\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the plan\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the plan\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who created the plan\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the plan was created\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"description\": \"Policies applied to this plan\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"policyDefinitionId\": { \"type\": \"string\" },\n          \"configuration\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"organizationId\", \"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/json-schema/apiman-plan-schema.json
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open Source
title: Apiman Plan
---
