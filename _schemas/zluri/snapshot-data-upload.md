---
description: Payload for uploading snapshot entity data within an active sync session. Snapshot data represents the current state of entities.
layout: schema
name: Zluri Snapshot Data Upload
properties_list:
- description: 'The type of snapshot entity being uploaded. Dependencies: users must be synced before groups, group_users, and activities.'
  name: entity
  type: string
- description: Page number for this batch of data. Re-uploading the same page number overwrites previous data for that page.
  name: page
  type: integer
- description: Array of entity records. Maximum 1000 records per page.
  name: data
  type: array
provider_name: Zluri
provider_slug: zluri
schema_file: json-schema/snapshot-data-upload.json
slug: snapshot-data-upload
source_filename: snapshot-data-upload.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/snapshot-data-upload.json\",\n  \"title\": \"Zluri Snapshot Data Upload\",\n  \"description\": \"Payload for uploading snapshot entity data within an active sync session. Snapshot data represents the current state of entities.\",\n  \"type\": \"object\",\n  \"required\": [\"entity\", \"page\", \"data\"],\n  \"properties\": {\n    \"entity\": {\n      \"type\": \"string\",\n      \"description\": \"The type of snapshot entity being uploaded. Dependencies: users must be synced before groups, group_users, and activities.\",\n      \"enum\": [\n        \"users\",\n        \"applications\",\n        \"contracts\",\n        \"transactions\",\n        \"groups\",\n        \"group_users\",\n        \"roles\",\n        \"activities\"\n      ]\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\":\
  \ \"Page number for this batch of data. Re-uploading the same page number overwrites previous data for that page.\",\n      \"minimum\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of entity records. Maximum 1000 records per page.\",\n      \"maxItems\": 1000,\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/snapshot-data-upload.json
tags:
- Access Management
- SaaS Management
title: Zluri Snapshot Data Upload
---
