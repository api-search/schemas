---
description: ListResourceProfileArtifactsResponse schema from Amazon Macie API
layout: schema
name: ListResourceProfileArtifactsResponse
properties_list:
- description: ''
  name: artifacts
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-resource-profile-artifacts-response-schema.json
slug: amazon-macie-list-resource-profile-artifacts-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-resource-profile-artifacts-response-schema.json\",\n  \"title\": \"ListResourceProfileArtifactsResponse\",\n  \"description\": \"ListResourceProfileArtifactsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfResourceProfileArtifact\"\n        },\n        {\n          \"description\": \"<p>An array of objects, one for each of 1-100 S3 objects that Amazon Macie selected for analysis.</p> <p>If Macie has analyzed more than 100 objects in the bucket, Macie populates the array based on the value for the ResourceProfileArtifact.sensitive field for an object: true (sensitive), followed by false (not sensitive). Macie then populates any remaining items in the\
  \ array with information about objects where the value for the ResourceProfileArtifact.classificationResultStatus field is SKIPPED.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-resource-profile-artifacts-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListResourceProfileArtifactsResponse
---
