---
description: A request to perform an action on an AppSheet table.
layout: schema
name: Google AppSheet Action Request
properties_list:
- description: The action to perform on the table.
  name: Action
  type: string
- description: Properties for the action.
  name: Properties
  type: object
- description: The rows to operate on or filter criteria.
  name: Rows
  type: array
provider_name: Google AppSheet
provider_slug: google-appsheet
schema_file: json-schema/ActionRequest.json
slug: ActionRequest
source_filename: ActionRequest.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"ActionRequest.json\",\n  \"title\": \"Google AppSheet Action Request\",\n  \"description\": \"A request to perform an action on an AppSheet table.\",\n  \"type\": \"object\",\n  \"required\": [\"Action\", \"Properties\"],\n  \"properties\": {\n    \"Action\": {\n      \"type\": \"string\",\n      \"description\": \"The action to perform on the table.\",\n      \"enum\": [\"Add\", \"Delete\", \"Edit\", \"Find\"]\n    },\n    \"Properties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties for the action.\",\n      \"properties\": {\n        \"Locale\": {\n          \"type\": \"string\",\n          \"description\": \"The locale for the request.\"\n        },\n        \"Timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The timezone for the request.\"\n        }\n      }\n    },\n    \"Rows\": {\n      \"type\": \"array\",\n      \"description\": \"The\
  \ rows to operate on or filter criteria.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-appsheet/refs/heads/main/json-schema/ActionRequest.json
tags:
- Applications
- Data
- Google
- Low-Code
- No-Code
- Tables
title: Google AppSheet Action Request
---
