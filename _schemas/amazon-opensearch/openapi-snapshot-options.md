---
description: Specifies the time, in UTC format, when the service takes a daily automated snapshot of the specified Elasticsearch domain. Default value is <code>0</code> hours.
layout: schema
name: SnapshotOptions
properties_list:
- description: ''
  name: AutomatedSnapshotStartHour
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-snapshot-options-schema.json
slug: openapi-snapshot-options
source_filename: openapi-snapshot-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-snapshot-options-schema.json\",\n  \"title\": \"SnapshotOptions\",\n  \"description\": \"Specifies the time, in UTC format, when the service takes a daily automated snapshot of the specified Elasticsearch domain. Default value is <code>0</code> hours.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomatedSnapshotStartHour\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"Specifies the time, in UTC format, when the service takes a daily automated snapshot of the specified Elasticsearch domain. Default value is <code>0</code> hours.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-snapshot-options-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: SnapshotOptions
---
