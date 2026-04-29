---
description: The result of <code>DescribeDomainAutoTunes</code> request. See the <a href="https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html" target="_blank">Developer Guide</a> for more information.
layout: schema
name: DescribeDomainAutoTunesResponse
properties_list:
- description: ''
  name: AutoTunes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-domain-auto-tunes-response-schema.json
slug: openapi-describe-domain-auto-tunes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-domain-auto-tunes-response-schema.json\",\n  \"title\": \"DescribeDomainAutoTunesResponse\",\n  \"description\": \"The result of <code>DescribeDomainAutoTunes</code> request. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoTunes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneList\"\n        },\n        {\n          \"description\": \"Specifies the list of setting adjustments that Auto-Tune has made to the domain. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a>\
  \ for more information.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Specifies an identifier to allow retrieval of paginated results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-domain-auto-tunes-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeDomainAutoTunesResponse
---
