---
description: UpdateClassifierRequest schema from Amazon Glue API
layout: schema
name: UpdateClassifierRequest
properties_list:
- description: ''
  name: GrokClassifier
  type: object
- description: ''
  name: XMLClassifier
  type: object
- description: ''
  name: JsonClassifier
  type: object
- description: ''
  name: CsvClassifier
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-classifier-request-schema.json
slug: glue-update-classifier-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-classifier-request-schema.json\",\n  \"title\": \"UpdateClassifierRequest\",\n  \"description\": \"UpdateClassifierRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GrokClassifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateGrokClassifierRequest\"\n        },\n        {\n          \"description\": \"A <code>GrokClassifier</code> object with updated fields.\"\n        }\n      ]\n    },\n    \"XMLClassifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateXMLClassifierRequest\"\n        },\n        {\n          \"description\": \"An <code>XMLClassifier</code> object with updated fields.\"\n        }\n      ]\n    },\n    \"JsonClassifier\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/UpdateJsonClassifierRequest\"\n        },\n        {\n          \"description\": \"A <code>JsonClassifier</code> object with updated fields.\"\n        }\n      ]\n    },\n    \"CsvClassifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateCsvClassifierRequest\"\n        },\n        {\n          \"description\": \"A <code>CsvClassifier</code> object with updated fields.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-classifier-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateClassifierRequest
---
