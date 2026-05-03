---
description: A Zesty.io instance represents an individual content management site or application. Each instance is assigned a unique ZUID (Zesty Universal Identifier) upon creation and can be interacted with over HTTPS.
layout: schema
name: Zesty Instance
properties_list:
- description: The Zesty Universal Identifier for the instance.
  name: ZUID
  type: string
- description: The name of the instance.
  name: name
  type: string
- description: The ecosystem ZUID this instance belongs to.
  name: ecoZUID
  type: string
- description: The primary domain for the instance.
  name: domain
  type: string
- description: The blueprint used to create the instance.
  name: blueprint
  type: string
- description: Timestamp when the instance was created.
  name: createdAt
  type: string
- description: Timestamp when the instance was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/instance.json
slug: instance
source_filename: instance.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/instance.json\",\n  \"title\": \"Zesty Instance\",\n  \"description\": \"A Zesty.io instance represents an individual content management site or application. Each instance is assigned a unique ZUID (Zesty Universal Identifier) upon creation and can be interacted with over HTTPS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the instance.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the instance.\"\n    },\n    \"ecoZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The ecosystem ZUID this instance belongs to.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The primary domain for the instance.\"\n    },\n    \"blueprint\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The blueprint used to create the instance.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the instance was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the instance was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/instance.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Instance
---
