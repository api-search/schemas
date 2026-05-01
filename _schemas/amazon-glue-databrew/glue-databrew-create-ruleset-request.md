---
description: CreateRulesetRequest schema from Amazon Glue DataBrew API
layout: schema
name: CreateRulesetRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: TargetArn
  type: object
- description: ''
  name: Rules
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-create-ruleset-request-schema.json
slug: glue-databrew-create-ruleset-request
source_filename: glue-databrew-create-ruleset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-ruleset-request-schema.json\",\n  \"title\": \"CreateRulesetRequest\",\n  \"description\": \"CreateRulesetRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetName\"\n        },\n        {\n          \"description\": \"The name of the ruleset to be created. Valid characters are alphanumeric (A-Z, a-z, 0-9), hyphen (-), period (.), and space.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetDescription\"\n        },\n        {\n          \"description\": \"The description of the ruleset.\"\n        }\n      ]\n    },\n    \"TargetArn\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a resource (dataset) that the ruleset is associated with.\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleList\"\n        },\n        {\n          \"description\": \"A list of rules that are defined with the ruleset. A rule includes one or more checks to be validated on a DataBrew dataset.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags to apply to the ruleset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"TargetArn\",\n    \"Rules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-ruleset-request-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CreateRulesetRequest
---
