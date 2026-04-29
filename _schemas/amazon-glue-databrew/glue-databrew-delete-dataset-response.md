---
description: DeleteDatasetResponse schema from Amazon Glue DataBrew API
layout: schema
name: DeleteDatasetResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-delete-dataset-response-schema.json
slug: glue-databrew-delete-dataset-response
source_filename: glue-databrew-delete-dataset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-delete-dataset-response-schema.json\",\n  \"title\": \"DeleteDatasetResponse\",\n  \"description\": \"DeleteDatasetResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\n        },\n        {\n          \"description\": \"The name of the dataset that you deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-delete-dataset-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DeleteDatasetResponse
---
