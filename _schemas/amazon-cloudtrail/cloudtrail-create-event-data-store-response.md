---
description: CreateEventDataStoreResponse schema
layout: schema
name: CreateEventDataStoreResponse
properties_list:
- description: ''
  name: EventDataStoreArn
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: RetentionPeriod
  type: integer
- description: ''
  name: CreatedTimestamp
  type: string
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-create-event-data-store-response-schema.json
slug: cloudtrail-create-event-data-store-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-event-data-store-response-schema.json\",\n  \"title\": \"CreateEventDataStoreResponse\",\n  \"description\": \"CreateEventDataStoreResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventDataStoreArn\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"RetentionPeriod\": {\n      \"type\": \"integer\"\n    },\n    \"CreatedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-event-data-store-response-schema.json
tags:
- AWS
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: CreateEventDataStoreResponse
---
