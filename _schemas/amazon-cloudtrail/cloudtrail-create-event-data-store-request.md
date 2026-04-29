---
description: CreateEventDataStoreRequest schema
layout: schema
name: CreateEventDataStoreRequest
properties_list:
- description: The name of the event data store.
  name: Name
  type: string
- description: Retention period in days.
  name: RetentionPeriod
  type: integer
- description: ''
  name: MultiRegionEnabled
  type: boolean
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-create-event-data-store-request-schema.json
slug: cloudtrail-create-event-data-store-request
source_filename: cloudtrail-create-event-data-store-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-event-data-store-request-schema.json\",\n  \"title\": \"CreateEventDataStoreRequest\",\n  \"description\": \"CreateEventDataStoreRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event data store.\"\n    },\n    \"RetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Retention period in days.\"\n    },\n    \"MultiRegionEnabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-event-data-store-request-schema.json
tags:
- AWS
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: CreateEventDataStoreRequest
---
