---
description: ListModelsResponse schema from Amazon Lookout for Vision API
layout: schema
name: ListModelsResponse
properties_list:
- description: ''
  name: Models
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-list-models-response-schema.json
slug: amazon-lookout-for-vision-list-models-response
source_filename: amazon-lookout-for-vision-list-models-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-models-response-schema.json\",\n  \"title\": \"ListModelsResponse\",\n  \"description\": \"ListModelsResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Models\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelMetadataList\"\n        },\n        {\n          \"description\": \"A list of model versions in the specified project. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the response is truncated, Amazon Lookout for Vision returns this token that you can use in the subsequent request to retrieve the next set of models.\
  \ \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-models-response-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ListModelsResponse
---
