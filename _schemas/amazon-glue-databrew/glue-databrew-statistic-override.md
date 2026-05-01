---
description: Override of a particular evaluation for a profile job.
layout: schema
name: StatisticOverride
properties_list:
- description: ''
  name: Statistic
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-statistic-override-schema.json
slug: glue-databrew-statistic-override
source_filename: glue-databrew-statistic-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-statistic-override-schema.json\",\n  \"title\": \"StatisticOverride\",\n  \"description\": \"Override of a particular evaluation for a profile job. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statistic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Statistic\"\n        },\n        {\n          \"description\": \"The name of an evaluation\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParameterMap\"\n        },\n        {\n          \"description\": \"A map that includes overrides of an evaluation\\u2019s parameters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Statistic\",\n    \"Parameters\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-statistic-override-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: StatisticOverride
---
