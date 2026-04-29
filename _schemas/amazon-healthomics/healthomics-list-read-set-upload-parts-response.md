---
description: ''
layout: schema
name: ListReadSetUploadPartsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: parts
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-read-set-upload-parts-response-schema.json
slug: healthomics-list-read-set-upload-parts-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-upload-parts-response-schema.json\",\n  \"title\": \"ListReadSetUploadPartsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" Next token returned in the response of a previous ListReadSetUploadParts call. Used to get the next page of results. \"\n        }\n      ]\n    },\n    \"parts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetUploadPartList\"\n        },\n        {\n          \"description\": \" An array of upload parts. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-upload-parts-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReadSetUploadPartsResponse
---
