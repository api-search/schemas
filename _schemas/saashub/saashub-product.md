---
description: Schema for a software product listing on the SaaSHub discovery platform
layout: schema
name: SaaSHub Product
properties_list:
- description: Unique product identifier (slug) on SaaSHub
  name: id
  type: string
- description: JSON:API resource type
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: SaaSHub
provider_slug: saashub
schema_file: json-schema/saashub-product-schema.json
slug: saashub-product
source_filename: saashub-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/saashub/refs/heads/main/json-schema/saashub-product-schema.json\",\n  \"title\": \"SaaSHub Product\",\n  \"description\": \"Schema for a software product listing on the SaaSHub discovery platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier (slug) on SaaSHub\",\n      \"example\": \"basecamp\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"products\",\n      \"description\": \"JSON:API resource type\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Official product name\",\n          \"example\": \"Basecamp\"\n        },\n        \"saashubUrl\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"uri\",\n          \"description\": \"Canonical SaaSHub listing URL\",\n          \"example\": \"https://www.saashub.com/basecamp\"\n        },\n        \"tagline\": {\n          \"type\": \"string\",\n          \"description\": \"Short product tagline or description\",\n          \"example\": \"The all-in-one toolkit for working remotely\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Product lifecycle status\",\n          \"enum\": [\"active\", \"discontinued\"],\n          \"example\": \"active\"\n        },\n        \"websiteUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Official product website URL\",\n          \"example\": \"https://basecamp.com\"\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Primary software category\",\n          \"example\": \"Project Management\"\n        },\n        \"categories\": {\n        \
  \  \"type\": \"array\",\n          \"description\": \"All categories the product belongs to\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": [\"Project Management\", \"Team Collaboration\"]\n        },\n        \"pricing\": {\n          \"type\": \"string\",\n          \"description\": \"Pricing model description\",\n          \"example\": \"Paid with free trial\"\n        },\n        \"license\": {\n          \"type\": \"string\",\n          \"description\": \"Software license type\",\n          \"example\": \"Proprietary\"\n        },\n        \"openSource\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the software is open source\"\n        },\n        \"upvoteCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of upvotes on SaaSHub\",\n          \"minimum\": 0\n        },\n        \"alternativeCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number\
  \ of alternatives listed on SaaSHub\",\n          \"minimum\": 0\n        }\n      },\n      \"required\": [\"name\", \"saashubUrl\", \"tagline\"]\n    }\n  },\n  \"required\": [\"id\", \"type\", \"attributes\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/saashub/refs/heads/main/json-schema/saashub-product-schema.json
tags:
- Alternatives
- SaaS
- Software Discovery
- Software Catalog
title: SaaSHub Product
---
