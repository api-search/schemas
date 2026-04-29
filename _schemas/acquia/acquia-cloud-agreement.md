---
description: agreement schema from Acquia Cloud API
layout: schema
name: Agreement
properties_list:
- description: The agreement UUID.
  name: uuid
  type: string
- description: The agreement document UUID.
  name: document_uuid
  type: string
- description: The name of the agreement.
  name: title
  type: string
- description: The formatted agreement content.
  name: body
  type: string
- description: The status of the agreement.
  name: status
  type: string
- description: The date the agreement was created.
  name: created_at
  type: string
- description: The date the agreement was last updated.
  name: updated_at
  type: string
- description: ''
  name: actioned_by
  type: object
- description: A reference to the entity for this agreement.
  name: reference
  type: object
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-agreement-schema.json
slug: acquia-cloud-agreement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-agreement-schema.json\",\n  \"title\": \"Agreement\",\n  \"description\": \"agreement schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The agreement UUID.\"\n    },\n    \"document_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The agreement document UUID.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the agreement.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The formatted agreement content.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the agreement.\",\n      \"enum\": [\n        \"pending\"\
  ,\n        \"accepted\",\n        \"declined\"\n      ]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the agreement was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the agreement was last updated.\",\n      \"nullable\": true\n    },\n    \"actioned_by\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-stub-nullable\"\n    },\n    \"reference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to the entity for this agreement.\",\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The entity UUID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The entity name.\"\n        },\n        \"type\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The entity type.\"\n        }\n      }\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"document_uuid\",\n    \"title\",\n    \"body\",\n    \"status\",\n    \"created_at\",\n    \"updated_at\",\n    \"actioned_by\",\n    \"reference\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-agreement-schema.json
tags:
- Content
- Experience
title: Agreement
---
