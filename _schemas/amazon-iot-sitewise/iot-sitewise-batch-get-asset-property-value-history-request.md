---
description: BatchGetAssetPropertyValueHistoryRequest schema
layout: schema
name: BatchGetAssetPropertyValueHistoryRequest
properties_list:
- description: ''
  name: entries
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-history-request-schema.json
slug: iot-sitewise-batch-get-asset-property-value-history-request
source_filename: iot-sitewise-batch-get-asset-property-value-history-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-request-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueHistoryRequest\",\n  \"description\": \"BatchGetAssetPropertyValueHistoryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueHistoryEntries\"\n        },\n        {\n          \"description\": \"The list of asset property historical value entries for the batch get request. You can specify up to 16 entries per request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to be used for the next set of paginated\
  \ results.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueHistoryMaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results to return for each paginated request. A result set is returned in the two cases, whichever occurs first.</p> <ul> <li> <p>The size of the result set is equal to 4 MB.</p> </li> <li> <p>The number of data points in the result set is equal to the value of <code>maxResults</code>. The maximum value of <code>maxResults</code> is 20000.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-history-request-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueHistoryRequest
---
