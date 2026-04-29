---
description: ide schema from Acquia Cloud API
layout: schema
name: Ide
properties_list:
- description: The unique identifier of the Cloud IDE.
  name: uuid
  type: string
- description: The human-friendly label of the Cloud IDE.
  name: label
  type: string
- description: The current provisioning status of the Cloud IDE.
  name: status
  type: string
- description: ''
  name: _links
  type: object
- description: ''
  name: _embedded
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-ide-schema.json
slug: acquia-cloud-ide
source_filename: acquia-cloud-ide-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-ide-schema.json\",\n  \"title\": \"Ide\",\n  \"description\": \"ide schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the Cloud IDE.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-friendly label of the Cloud IDE.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current provisioning status of the Cloud IDE.\",\n      \"enum\": [\n        \"active\",\n        \"provisioning\",\n        \"deleting\",\n        \"updating\",\n        \"provision-failed\",\n        \"update-failed\",\n        \"delete-failed\"\n      ]\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\
  \n    },\n    \"_embedded\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"owner\": {\n          \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-profile\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"label\",\n    \"status\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-ide-schema.json
tags:
- Content
- Experience
title: Ide
---
