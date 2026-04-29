---
description: Container for the parameters to the <code><a>CancelElasticsearchServiceSoftwareUpdate</a></code> operation. Specifies the name of the Elasticsearch domain that you wish to cancel a service software update on.
layout: schema
name: CancelElasticsearchServiceSoftwareUpdateRequest
properties_list:
- description: ''
  name: DomainName
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-cancel-elasticsearch-service-software-update-request-schema.json
slug: openapi-cancel-elasticsearch-service-software-update-request
source_filename: openapi-cancel-elasticsearch-service-software-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-cancel-elasticsearch-service-software-update-request-schema.json\",\n  \"title\": \"CancelElasticsearchServiceSoftwareUpdateRequest\",\n  \"description\": \"Container for the parameters to the <code><a>CancelElasticsearchServiceSoftwareUpdate</a></code> operation. Specifies the name of the Elasticsearch domain that you wish to cancel a service software update on.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that you want to stop the latest service software update on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-cancel-elasticsearch-service-software-update-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CancelElasticsearchServiceSoftwareUpdateRequest
---
