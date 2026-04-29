---
description: Configuration of statistics that are allowed to be run on columns that contain detected entities. When undefined, no statistics will be computed on columns that contain detected entities.
layout: schema
name: AllowedStatistics
properties_list:
- description: ''
  name: Statistics
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-allowed-statistics-schema.json
slug: glue-databrew-allowed-statistics
source_filename: glue-databrew-allowed-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-allowed-statistics-schema.json\",\n  \"title\": \"AllowedStatistics\",\n  \"description\": \"Configuration of statistics that are allowed to be run on columns that contain detected entities. When undefined, no statistics will be computed on columns that contain detected entities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatisticList\"\n        },\n        {\n          \"description\": \"One or more column statistics to allow for columns that contain detected entities.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Statistics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-allowed-statistics-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: AllowedStatistics
---
