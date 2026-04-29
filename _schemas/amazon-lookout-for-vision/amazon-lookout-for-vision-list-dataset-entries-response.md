---
description: ListDatasetEntriesResponse schema from Amazon Lookout for Vision API
layout: schema
name: ListDatasetEntriesResponse
properties_list:
- description: ''
  name: DatasetEntries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-list-dataset-entries-response-schema.json
slug: amazon-lookout-for-vision-list-dataset-entries-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-dataset-entries-response-schema.json\",\n  \"title\": \"ListDatasetEntriesResponse\",\n  \"description\": \"ListDatasetEntriesResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetEntryList\"\n        },\n        {\n          \"description\": \"A list of the entries (JSON Lines) within the dataset.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the response is truncated, Amazon Lookout for Vision returns this token that you can use in the subsequent request to\
  \ retrieve the next set ofdataset entries.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-dataset-entries-response-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ListDatasetEntriesResponse
---
