---
description: ListResourceProfileDetectionsResponse schema from Amazon Macie API
layout: schema
name: ListResourceProfileDetectionsResponse
properties_list:
- description: ''
  name: detections
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-resource-profile-detections-response-schema.json
slug: amazon-macie-list-resource-profile-detections-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-resource-profile-detections-response-schema.json\",\n  \"title\": \"ListResourceProfileDetectionsResponse\",\n  \"description\": \"ListResourceProfileDetectionsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfDetection\"\n        },\n        {\n          \"description\": \"An array of objects, one for each type of sensitive data that Amazon Macie found in the bucket. Each object reports the number of occurrences of the specified type and provides information about the custom data identifier or managed data identifier that detected the data.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-resource-profile-detections-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListResourceProfileDetectionsResponse
---
