---
description: ListEventDataStoresResponse schema
layout: schema
name: ListEventDataStoresResponse
properties_list:
- description: ''
  name: EventDataStores
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-list-event-data-stores-response-schema.json
slug: cloudtrail-list-event-data-stores-response
source_filename: cloudtrail-list-event-data-stores-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-list-event-data-stores-response-schema.json\",\n  \"title\": \"ListEventDataStoresResponse\",\n  \"description\": \"ListEventDataStoresResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventDataStores\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"EventDataStoreArn\": {\n            \"type\": \"string\"\n          },\n          \"Name\": {\n            \"type\": \"string\"\n          },\n          \"Status\": {\n            \"type\": \"string\"\n          },\n          \"RetentionPeriod\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-list-event-data-stores-response-schema.json
tags:
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: ListEventDataStoresResponse
---
