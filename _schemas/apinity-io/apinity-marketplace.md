---
description: Schema representing an API registered in the Apinity compliant API marketplace
layout: schema
name: Apinity Marketplace API
properties_list:
- description: Unique identifier for the marketplace API
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API and its capabilities
  name: description
  type: string
- description: Organization providing the API
  name: provider
  type: string
- description: API version
  name: version
  type: string
- description: Lifecycle status of the API in the marketplace
  name: status
  type: string
- description: Compliance policies applied to this API
  name: compliancePolicies
  type: array
- description: Categories classifying this API in the marketplace
  name: categories
  type: array
- description: Timestamp when the API was registered in the marketplace
  name: createdAt
  type: string
provider_name: Apinity.io
provider_slug: apinity-io
schema_file: json-schema/apinity-marketplace-schema.json
slug: apinity-marketplace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apinity-io/main/json-schema/apinity-marketplace-schema.json\",\n  \"title\": \"Apinity Marketplace API\",\n  \"description\": \"Schema representing an API registered in the Apinity compliant API marketplace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the marketplace API\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API and its capabilities\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"Organization providing the API\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\"draft\", \"published\", \"deprecated\", \"retired\"],\n      \"description\": \"Lifecycle status of the API in the marketplace\"\n    },\n    \"compliancePolicies\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Compliance policies applied to this API\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Categories classifying this API in the marketplace\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was registered in the marketplace\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"provider\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apinity-io/refs/heads/main/json-schema/apinity-marketplace-schema.json
tags:
- API Governance
- API Marketplace
- Compliance
- Discovery
- Integration Platform
title: Apinity Marketplace API
---
