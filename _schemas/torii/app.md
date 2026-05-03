---
description: An application discovered and tracked within the Torii SaaS Management Platform.
layout: schema
name: Torii App
properties_list:
- description: Unique identifier for the app.
  name: id
  type: string
- description: Name of the application.
  name: name
  type: string
- description: Application category.
  name: category
  type: string
- description: Current state (e.g. discovered, managed, closed).
  name: state
  type: string
- description: Application URL.
  name: url
  type: string
- description: Number of active users.
  name: activeUsers
  type: integer
- description: Total number of users.
  name: totalUsers
  type: integer
- description: Total number of licenses.
  name: totalLicenses
  type: integer
- description: Annual cost of the application.
  name: annualCost
  type: number
- description: Application owner.
  name: owner
  type: string
- description: When the app was first discovered.
  name: createdAt
  type: string
provider_name: Torii
provider_slug: torii
schema_file: json-schema/app.json
slug: app
source_filename: app.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/app.json\",\n  \"title\": \"Torii App\",\n  \"description\": \"An application discovered and tracked within the Torii SaaS Management Platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the app.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Application category.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state (e.g. discovered, managed, closed).\",\n      \"enum\": [\"discovered\", \"managed\", \"closed\"]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Application\
  \ URL.\"\n    },\n    \"activeUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active users.\"\n    },\n    \"totalUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of users.\"\n    },\n    \"totalLicenses\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of licenses.\"\n    },\n    \"annualCost\": {\n      \"type\": \"number\",\n      \"description\": \"Annual cost of the application.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Application owner.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the app was first discovered.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/app.json
tags:
- SaaS Management
title: Torii App
---
