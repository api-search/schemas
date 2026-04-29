---
description: The result of a <code>StartElasticsearchServiceSoftwareUpdate</code> operation. Contains the status of the update.
layout: schema
name: StartElasticsearchServiceSoftwareUpdateResponse
properties_list:
- description: ''
  name: ServiceSoftwareOptions
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-start-elasticsearch-service-software-update-response-schema.json
slug: openapi-start-elasticsearch-service-software-update-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-start-elasticsearch-service-software-update-response-schema.json\",\n  \"title\": \"StartElasticsearchServiceSoftwareUpdateResponse\",\n  \"description\": \"The result of a <code>StartElasticsearchServiceSoftwareUpdate</code> operation. Contains the status of the update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceSoftwareOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceSoftwareOptions\"\n        },\n        {\n          \"description\": \"The current status of the Elasticsearch service software update.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-start-elasticsearch-service-software-update-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: StartElasticsearchServiceSoftwareUpdateResponse
---
