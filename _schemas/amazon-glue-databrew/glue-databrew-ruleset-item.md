---
description: Contains metadata about the ruleset.
layout: schema
name: RulesetItem
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: CreateDate
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: RuleCount
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: TargetArn
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-ruleset-item-schema.json
slug: glue-databrew-ruleset-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-ruleset-item-schema.json\",\n  \"title\": \"RulesetItem\",\n  \"description\": \"Contains metadata about the ruleset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the ruleset.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who created the ruleset.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n   \
  \     },\n        {\n          \"description\": \"The date and time that the ruleset was created.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetDescription\"\n        },\n        {\n          \"description\": \"The description of the ruleset.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who last modified the ruleset.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The modification date and time of the ruleset.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetName\"\n        },\n\
  \        {\n          \"description\": \"The name of the ruleset.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the ruleset.\"\n        }\n      ]\n    },\n    \"RuleCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleCount\"\n        },\n        {\n          \"description\": \"The number of rules that are defined in the ruleset.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags that have been applied to the ruleset.\"\n        }\n      ]\n    },\n    \"TargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN)\
  \ of a resource (dataset) that the ruleset is associated with.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"TargetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-ruleset-item-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: RulesetItem
---
