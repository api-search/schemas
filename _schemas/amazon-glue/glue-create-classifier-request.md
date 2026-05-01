---
description: CreateClassifierRequest schema from Amazon Glue API
layout: schema
name: CreateClassifierRequest
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
schema_file: json-schema/glue-create-classifier-request-schema.json
slug: glue-create-classifier-request
source_filename: glue-create-classifier-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-classifier-request-schema.json\",\n  \"title\": \"CreateClassifierRequest\",\n  \"description\": \"CreateClassifierRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GrokClassifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateGrokClassifierRequest\"\n        },\n        {\n          \"description\": \"A <code>GrokClassifier</code> object specifying the classifier to create.\"\n        }\n      ]\n    },\n    \"XMLClassifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateXMLClassifierRequest\"\n        },\n        {\n          \"description\": \"An <code>XMLClassifier</code> object specifying the classifier to create.\"\n        }\n      ]\n    },\n    \"JsonClassifier\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateJsonClassifierRequest\"\n        },\n        {\n          \"description\": \"A <code>JsonClassifier</code> object specifying the classifier to create.\"\n        }\n      ]\n    },\n    \"CsvClassifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateCsvClassifierRequest\"\n        },\n        {\n          \"description\": \"A <code>CsvClassifier</code> object specifying the classifier to create.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-classifier-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateClassifierRequest
---
