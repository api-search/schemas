---
description: SOAP envelope containing an entity element for the target schema with attribute values and an _operation attribute controlling the write behavior.
layout: schema
name: WriteRequest
properties_list:
- description: ''
  name: entity
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-write-request-schema.json
slug: adobe-campaign-classic-write-request
source_filename: adobe-campaign-classic-write-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-write-request-schema.json\",\n  \"title\": \"WriteRequest\",\n  \"description\": \"SOAP envelope containing an entity element for the target schema with attribute values and an _operation attribute controlling the write behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"_operation\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"insert\",\n            \"insertOrUpdate\",\n            \"update\",\n            \"delete\"\n          ],\n          \"description\": \"The write operation to perform. insert creates a new record, insertOrUpdate creates or updates, update modifies existing, delete removes.\"\n        },\n        \"_schema\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Target schema name.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-write-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: WriteRequest
---
