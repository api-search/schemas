---
description: Container for response returned by <code> <a>GetUpgradeHistory</a> </code> operation.
layout: schema
name: GetUpgradeHistoryResponse
properties_list:
- description: ''
  name: UpgradeHistories
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-get-upgrade-history-response-schema.json
slug: openapi-get-upgrade-history-response
source_filename: openapi-get-upgrade-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-upgrade-history-response-schema.json\",\n  \"title\": \"GetUpgradeHistoryResponse\",\n  \"description\": \" Container for response returned by <code> <a>GetUpgradeHistory</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpgradeHistories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeHistoryList\"\n        },\n        {\n          \"description\": \" A list of <code> <a>UpgradeHistory</a> </code> objects corresponding to each Upgrade or Upgrade Eligibility Check performed on a domain returned as part of <code> <a>GetUpgradeHistoryResponse</a> </code> object. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n  \
  \        \"description\": \"Pagination token that needs to be supplied to the next call to get the next page of results\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-upgrade-history-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: GetUpgradeHistoryResponse
---
