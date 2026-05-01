---
description: BatchGetAssetPropertyValueResponse schema
layout: schema
name: BatchGetAssetPropertyValueResponse
properties_list:
- description: ''
  name: errorEntries
  type: object
- description: ''
  name: successEntries
  type: object
- description: ''
  name: skippedEntries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-response-schema.json
slug: iot-sitewise-batch-get-asset-property-value-response
source_filename: iot-sitewise-batch-get-asset-property-value-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-response-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueResponse\",\n  \"description\": \"BatchGetAssetPropertyValueResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueErrorEntries\"\n        },\n        {\n          \"description\": \"A list of the errors (if any) associated with the batch request. Each error entry contains the <code>entryId</code> of the entry that failed.\"\n        }\n      ]\n    },\n    \"successEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueSuccessEntries\"\n        },\n        {\n          \"description\": \"A list of\
  \ entries that were processed successfully by this batch request. Each success entry contains the <code>entryId</code> of the entry that succeeded and the latest query result.\"\n        }\n      ]\n    },\n    \"skippedEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueSkippedEntries\"\n        },\n        {\n          \"description\": \"A list of entries that were not processed by this batch request. because these entries had been completely processed by previous paginated requests. Each skipped entry contains the <code>entryId</code> of the entry that skipped.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorEntries\",\n    \"successEntries\"\
  ,\n    \"skippedEntries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueResponse
---
