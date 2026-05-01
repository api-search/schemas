---
description: DescribeRulesetResponse schema from Amazon Glue DataBrew API
layout: schema
name: DescribeRulesetResponse
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
  name: CreateDate
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-describe-ruleset-response-schema.json
slug: glue-databrew-describe-ruleset-response
source_filename: glue-databrew-describe-ruleset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-ruleset-response-schema.json\",\n  \"title\": \"DescribeRulesetResponse\",\n  \"description\": \"DescribeRulesetResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetName\"\n        },\n        {\n          \"description\": \"The name of the ruleset.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetDescription\"\n        },\n        {\n          \"description\": \"The description of the ruleset.\"\n        }\n      ]\n    },\n    \"TargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n \
  \         \"description\": \"The Amazon Resource Name (ARN) of a resource (dataset) that the ruleset is associated with.\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleList\"\n        },\n        {\n          \"description\": \"A list of rules that are defined with the ruleset. A rule includes one or more checks to be validated on a DataBrew dataset.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the ruleset was created.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who created the ruleset.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who last modified the ruleset.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The modification date and time of the ruleset.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the ruleset.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags that have been applied to the ruleset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-ruleset-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DescribeRulesetResponse
---
