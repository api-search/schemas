---
description: Configuration for data quality validation. Used to select the Rulesets and Validation Mode to be used in the profile job. When ValidationConfiguration is null, the profile job will run without data quality validation.
layout: schema
name: ValidationConfiguration
properties_list:
- description: ''
  name: RulesetArn
  type: object
- description: ''
  name: ValidationMode
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-validation-configuration-schema.json
slug: glue-databrew-validation-configuration
source_filename: glue-databrew-validation-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-validation-configuration-schema.json\",\n  \"title\": \"ValidationConfiguration\",\n  \"description\": \"Configuration for data quality validation. Used to select the Rulesets and Validation Mode to be used in the profile job. When ValidationConfiguration is null, the profile job will run without data quality validation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RulesetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the ruleset to be validated in the profile job. The TargetArn of the selected ruleset should be the same as the Amazon Resource Name (ARN) of the dataset that is associated with the profile job.\"\n        }\n      ]\n    },\n   \
  \ \"ValidationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValidationMode\"\n        },\n        {\n          \"description\": \"Mode of data quality validation. Default mode is \\u201cCHECK_ALL\\u201d which verifies all rules defined in the selected ruleset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RulesetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-validation-configuration-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ValidationConfiguration
---
