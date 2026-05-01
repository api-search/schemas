---
description: Configuration of evaluations for a profile job. This configuration can be used to select evaluations and override the parameters of selected evaluations.
layout: schema
name: StatisticsConfiguration
properties_list:
- description: ''
  name: IncludedStatistics
  type: object
- description: ''
  name: Overrides
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-statistics-configuration-schema.json
slug: glue-databrew-statistics-configuration
source_filename: glue-databrew-statistics-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-statistics-configuration-schema.json\",\n  \"title\": \"StatisticsConfiguration\",\n  \"description\": \"Configuration of evaluations for a profile job. This configuration can be used to select evaluations and override the parameters of selected evaluations. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IncludedStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatisticList\"\n        },\n        {\n          \"description\": \"List of included evaluations. When the list is undefined, all supported evaluations will be included.\"\n        }\n      ]\n    },\n    \"Overrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatisticOverrideList\"\n        },\n        {\n          \"description\": \"List\
  \ of overrides for evaluations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-statistics-configuration-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: StatisticsConfiguration
---
