---
description: ''
layout: schema
name: ListDatastoresResponse
properties_list:
- description: ''
  name: datastoreSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-list-datastores-response-schema.json
slug: healthimaging-list-datastores-response
source_filename: healthimaging-list-datastores-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-list-datastores-response-schema.json\",\n  \"title\": \"ListDatastoresResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datastoreSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreSummaries\"\n        },\n        {\n          \"description\": \"The list of summaries of data stores.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the list of data stores on the next page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-list-datastores-response-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: ListDatastoresResponse
---
