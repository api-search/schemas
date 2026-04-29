---
description: Container for the parameters to the <code>DescribeDomainAutoTunes</code> operation.
layout: schema
name: DescribeDomainAutoTunesRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-domain-auto-tunes-request-schema.json
slug: openapi-describe-domain-auto-tunes-request
source_filename: openapi-describe-domain-auto-tunes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-domain-auto-tunes-request-schema.json\",\n  \"title\": \"DescribeDomainAutoTunesRequest\",\n  \"description\": \"Container for the parameters to the <code>DescribeDomainAutoTunes</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"Set this value to limit the number of results returned. If not specified, defaults to 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"NextToken is sent in case the earlier API call results contain the NextToken. It is used for pagination.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-domain-auto-tunes-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeDomainAutoTunesRequest
---
