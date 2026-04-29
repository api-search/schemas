---
description: Configuration for column evaluations for a profile job. ColumnStatisticsConfiguration can be used to select evaluations and override parameters of evaluations for particular columns.
layout: schema
name: ColumnStatisticsConfiguration
properties_list:
- description: ''
  name: Selectors
  type: object
- description: ''
  name: Statistics
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-column-statistics-configuration-schema.json
slug: glue-databrew-column-statistics-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-column-statistics-configuration-schema.json\",\n  \"title\": \"ColumnStatisticsConfiguration\",\n  \"description\": \"Configuration for column evaluations for a profile job. ColumnStatisticsConfiguration can be used to select evaluations and override parameters of evaluations for particular columns. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Selectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnSelectorList\"\n        },\n        {\n          \"description\": \"List of column selectors. Selectors can be used to select columns from the dataset. When selectors are undefined, configuration will be applied to all supported columns. \"\n        }\n      ]\n    },\n    \"Statistics\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/StatisticsConfiguration\"\n        },\n        {\n          \"description\": \"Configuration for evaluations. Statistics can be used to select evaluations and override parameters of evaluations. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Statistics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-column-statistics-configuration-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ColumnStatisticsConfiguration
---
