---
description: The configured log publishing options for the domain and their current status.
layout: schema
name: LogPublishingOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-log-publishing-options-status-schema.json
slug: openapi-log-publishing-options-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-log-publishing-options-status-schema.json\",\n  \"title\": \"LogPublishingOptionsStatus\",\n  \"description\": \"The configured log publishing options for the domain and their current status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogPublishingOptions\"\n        },\n        {\n          \"description\": \"The log publishing options configured for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \"The status of the log publishing options for the Elasticsearch domain. See <code>OptionStatus</code> for the status information that's\
  \ included. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-log-publishing-options-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: LogPublishingOptionsStatus
---
