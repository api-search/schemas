---
description: Details about the last operation performed on the service instance.
layout: schema
name: LastOperation
properties_list:
- description: The type of operation that was performed.
  name: type
  type: string
- description: The current state of the operation.
  name: state
  type: string
- description: A human-readable description of the operation status.
  name: description
  type: string
- description: ISO 8601 timestamp when the operation was initiated.
  name: created_at
  type: string
- description: ISO 8601 timestamp when the operation status was last updated.
  name: updated_at
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-last-operation-schema.json
slug: sap-hana-cloud-rest-last-operation
source_filename: sap-hana-cloud-rest-last-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LastOperation\",\n  \"type\": \"object\",\n  \"description\": \"Details about the last operation performed on the service instance.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of operation that was performed.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the operation.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the operation status.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the operation was initiated.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the operation status was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-last-operation-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: LastOperation
---
