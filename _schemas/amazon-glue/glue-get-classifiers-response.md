---
description: GetClassifiersResponse schema from Amazon Glue API
layout: schema
name: GetClassifiersResponse
properties_list:
- description: ''
  name: Classifiers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-classifiers-response-schema.json
slug: glue-get-classifiers-response
source_filename: glue-get-classifiers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-classifiers-response-schema.json\",\n  \"title\": \"GetClassifiersResponse\",\n  \"description\": \"GetClassifiersResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Classifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassifierList\"\n        },\n        {\n          \"description\": \"The requested list of classifier objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-classifiers-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetClassifiersResponse
---
