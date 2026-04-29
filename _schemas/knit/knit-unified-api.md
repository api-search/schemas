---
description: JSON Schema for Knit Unified API resources.
layout: schema
name: Knit Unified API Resources
properties_list: []
provider_name: Knit
provider_slug: knit
schema_file: json-schema/knit-unified-api-schema.json
slug: knit-unified-api
source_filename: knit-unified-api-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/knit/json-schema/knit-unified-api-schema.json\",\n  \"title\": \"Knit Unified API Resources\",\n  \"description\": \"JSON Schema for Knit Unified API resources.\",\n  \"definitions\": {\n    \"Employee\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"first_name\": { \"type\": \"string\" },\n        \"last_name\": { \"type\": \"string\" },\n        \"email\": { \"type\": \"string\", \"format\": \"email\" },\n        \"job_title\": { \"type\": \"string\" },\n        \"department\": { \"type\": \"string\" },\n        \"location\": { \"type\": \"string\" },\n        \"employment_status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"inactive\", \"terminated\"]\n        },\n        \"start_date\": { \"type\": \"string\", \"format\": \"date\" },\n        \"termination_date\": {\
  \ \"type\": [\"string\", \"null\"], \"format\": \"date\" },\n        \"manager_id\": { \"type\": [\"string\", \"null\"] },\n        \"integration_id\": { \"type\": \"string\" }\n      },\n      \"required\": [\"id\", \"first_name\", \"last_name\"]\n    },\n    \"Department\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"parent_id\": { \"type\": [\"string\", \"null\"] },\n        \"integration_id\": { \"type\": \"string\" }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"Location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"address\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" },\n        \"integration_id\": { \"type\": \"string\" }\n\
  \      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"TimeOff\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"employee_id\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\" },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"pending\", \"approved\", \"denied\", \"cancelled\"]\n        },\n        \"start_date\": { \"type\": \"string\", \"format\": \"date\" },\n        \"end_date\": { \"type\": \"string\", \"format\": \"date\" },\n        \"integration_id\": { \"type\": \"string\" }\n      },\n      \"required\": [\"id\", \"employee_id\"]\n    },\n    \"Integration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"provider\": { \"type\": \"string\" },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"inactive\", \"error\"]\n        },\n        \"created_at\"\
  : { \"type\": \"string\", \"format\": \"date-time\" },\n        \"last_synced_at\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" }\n      },\n      \"required\": [\"id\", \"provider\"]\n    },\n    \"Pagination\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"page\": { \"type\": \"integer\" },\n        \"page_size\": { \"type\": \"integer\" },\n        \"total_count\": { \"type\": \"integer\" },\n        \"total_pages\": { \"type\": \"integer\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/knit/refs/heads/main/json-schema/knit-unified-api-schema.json
tags:
- B2B
- HR Integrations
- HRIS
- Unified API
title: Knit Unified API Resources
---
