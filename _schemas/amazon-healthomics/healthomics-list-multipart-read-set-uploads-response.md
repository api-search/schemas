---
description: ''
layout: schema
name: ListMultipartReadSetUploadsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: uploads
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-multipart-read-set-uploads-response-schema.json
slug: healthomics-list-multipart-read-set-uploads-response
source_filename: healthomics-list-multipart-read-set-uploads-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-multipart-read-set-uploads-response-schema.json\",\n  \"title\": \"ListMultipartReadSetUploadsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" Next token returned in the response of a previous ListMultipartReadSetUploads call. Used to get the next page of results. \"\n        }\n      ]\n    },\n    \"uploads\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultipartReadSetUploadList\"\n        },\n        {\n          \"description\": \" An array of multipart uploads. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-multipart-read-set-uploads-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListMultipartReadSetUploadsResponse
---
