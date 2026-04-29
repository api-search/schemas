---
description: The result of a <code>DescribeDomainChangeProgress</code> request. Contains the progress information of the requested domain change.
layout: schema
name: DescribeDomainChangeProgressResponse
properties_list:
- description: ''
  name: ChangeProgressStatus
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-domain-change-progress-response-schema.json
slug: openapi-describe-domain-change-progress-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-domain-change-progress-response-schema.json\",\n  \"title\": \"DescribeDomainChangeProgressResponse\",\n  \"description\": \"The result of a <code>DescribeDomainChangeProgress</code> request. Contains the progress information of the requested domain change. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeProgressStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeProgressStatusDetails\"\n        },\n        {\n          \"description\": \"Progress information for the configuration change that is requested in the <code>DescribeDomainChangeProgress</code> request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-domain-change-progress-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeDomainChangeProgressResponse
---
