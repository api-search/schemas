---
description: Schema representing an API managed by the Apiman API management platform
layout: schema
name: Apiman API
properties_list:
- description: Organization identifier owning this API
  name: organizationId
  type: string
- description: Unique identifier for the API
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API
  name: description
  type: string
- description: Username of the user who created the API
  name: createdBy
  type: string
- description: Timestamp when the API was created
  name: createdOn
  type: string
- description: Number of published versions of this API
  name: numPublished
  type: integer
- description: Tags associated with the API
  name: tags
  type: array
provider_name: Apiman
provider_slug: apiman
schema_file: json-schema/apiman-api-schema.json
slug: apiman-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apiman/main/json-schema/apiman-api-schema.json\",\n  \"title\": \"Apiman API\",\n  \"description\": \"Schema representing an API managed by the Apiman API management platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization identifier owning this API\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who created the API\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was created\"\n    },\n    \"numPublished\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of published versions of this API\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Tags associated with the API\"\n    }\n  },\n  \"required\": [\"organizationId\", \"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/json-schema/apiman-api-schema.json
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open Source
title: Apiman API
---
