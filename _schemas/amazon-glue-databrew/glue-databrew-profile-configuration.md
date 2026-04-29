---
description: Configuration for profile jobs. Configuration can be used to select columns, do evaluations, and override default parameters of evaluations. When configuration is undefined, the profile job will apply default settings to all supported columns.
layout: schema
name: ProfileConfiguration
properties_list:
- description: ''
  name: DatasetStatisticsConfiguration
  type: object
- description: ''
  name: ProfileColumns
  type: object
- description: ''
  name: ColumnStatisticsConfigurations
  type: object
- description: ''
  name: EntityDetectorConfiguration
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-profile-configuration-schema.json
slug: glue-databrew-profile-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-profile-configuration-schema.json\",\n  \"title\": \"ProfileConfiguration\",\n  \"description\": \"Configuration for profile jobs. Configuration can be used to select columns, do evaluations, and override default parameters of evaluations. When configuration is undefined, the profile job will apply default settings to all supported columns. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetStatisticsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatisticsConfiguration\"\n        },\n        {\n          \"description\": \"Configuration for inter-column evaluations. Configuration can be used to select evaluations and override parameters of evaluations. When configuration is undefined, the profile job will run all supported\
  \ inter-column evaluations. \"\n        }\n      ]\n    },\n    \"ProfileColumns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnSelectorList\"\n        },\n        {\n          \"description\": \"List of column selectors. ProfileColumns can be used to select columns from the dataset. When ProfileColumns is undefined, the profile job will profile all supported columns. \"\n        }\n      ]\n    },\n    \"ColumnStatisticsConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnStatisticsConfigurationList\"\n        },\n        {\n          \"description\": \"List of configurations for column evaluations. ColumnStatisticsConfigurations are used to select evaluations and override parameters of evaluations for particular columns. When ColumnStatisticsConfigurations is undefined, the profile job will profile all supported columns and run all supported evaluations. \"\n        }\n      ]\n    },\n    \"EntityDetectorConfiguration\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDetectorConfiguration\"\n        },\n        {\n          \"description\": \"Configuration of entity detection for a profile job. When undefined, entity detection is disabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-profile-configuration-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ProfileConfiguration
---
