---
description: SOAP envelope containing a collection of entity elements for batch write operations. Each entity can specify its own _operation.
layout: schema
name: WriteCollectionRequest
properties_list:
- description: ''
  name: collection
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-write-collection-request-schema.json
slug: adobe-campaign-classic-write-collection-request
source_filename: adobe-campaign-classic-write-collection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-write-collection-request-schema.json\",\n  \"title\": \"WriteCollectionRequest\",\n  \"description\": \"SOAP envelope containing a collection of entity elements for batch write operations. Each entity can specify its own _operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"collection\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"_schema\": {\n          \"type\": \"string\",\n          \"description\": \"Target schema name for all entities.\"\n        },\n        \"entities\": {\n          \"type\": \"array\",\n          \"description\": \"Array of entity elements to write.\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-write-collection-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: WriteCollectionRequest
---
