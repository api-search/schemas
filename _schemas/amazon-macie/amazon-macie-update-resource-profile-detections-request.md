---
description: UpdateResourceProfileDetectionsRequest schema from Amazon Macie API
layout: schema
name: UpdateResourceProfileDetectionsRequest
properties_list:
- description: ''
  name: suppressDataIdentifiers
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-resource-profile-detections-request-schema.json
slug: amazon-macie-update-resource-profile-detections-request
source_filename: amazon-macie-update-resource-profile-detections-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-resource-profile-detections-request-schema.json\",\n  \"title\": \"UpdateResourceProfileDetectionsRequest\",\n  \"description\": \"UpdateResourceProfileDetectionsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"suppressDataIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSuppressDataIdentifier\"\n        },\n        {\n          \"description\": \"An array of objects, one for each custom data identifier or managed data identifier that detected the type of sensitive data to start excluding or including in the bucket's score. To start including all sensitive data types in the score, don't specify any values for this array.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-resource-profile-detections-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateResourceProfileDetectionsRequest
---
