---
description: An application represents a SaaS software product tracked within the Zylo platform, including metadata such as owner, category, spend, and custom fields.
layout: schema
name: Zylo Application
properties_list:
- description: The unique identifier of the application.
  name: id
  type: string
- description: The display name of the application.
  name: name
  type: string
- description: The category of the application.
  name: category
  type: string
- description: The owner of the application.
  name: owner
  type: string
- description: The current status of the application.
  name: status
  type: string
- description: Whether the application is marked for true-up.
  name: trueUp
  type: boolean
- description: The total spend on this application.
  name: totalSpend
  type: number
- description: The number of subscriptions for this application.
  name: subscriptionCount
  type: integer
- description: The date and time the application was created.
  name: createdAt
  type: string
- description: The date and time the application was last updated.
  name: updatedAt
  type: string
- description: Custom fields associated with the application.
  name: customFields
  type: object
provider_name: Zylo
provider_slug: zylo
schema_file: json-schema/application.json
slug: application
source_filename: application.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"application.json\",\n  \"title\": \"Zylo Application\",\n  \"description\": \"An application represents a SaaS software product tracked within the Zylo platform, including metadata such as owner, category, spend, and custom fields.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the application.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the application.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The owner of the application.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the application.\",\n      \"enum\": [\"active\", \"inactive\"\
  , \"under_review\"]\n    },\n    \"trueUp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application is marked for true-up.\"\n    },\n    \"totalSpend\": {\n      \"type\": \"number\",\n      \"description\": \"The total spend on this application.\"\n    },\n    \"subscriptionCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of subscriptions for this application.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the application was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the application was last updated.\"\n    },\n    \"customFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom fields associated with the application.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"status\"\
  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/json-schema/application.json
tags:
- Budgets
- SaaS Management
- Spend
title: Zylo Application
---
