---
description: ListDataSetImportHistoryResponse schema from AWS Mainframe Modernization API
layout: schema
name: ListDataSetImportHistoryResponse
properties_list:
- description: ''
  name: dataSetImportTasks
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-list-data-set-import-history-response-schema.json
slug: amazon-mainframe-modernization-list-data-set-import-history-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-data-set-import-history-response-schema.json\",\n  \"title\": \"ListDataSetImportHistoryResponse\",\n  \"description\": \"ListDataSetImportHistoryResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSetImportTasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSetImportTaskList\"\n        },\n        {\n          \"description\": \"The data set import tasks.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If there are more items to return, this contains a token that is passed to a subsequent call to this operation to\
  \ retrieve the next set of items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dataSetImportTasks\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-data-set-import-history-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ListDataSetImportHistoryResponse
---
