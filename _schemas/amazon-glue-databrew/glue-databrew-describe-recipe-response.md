---
description: DescribeRecipeResponse schema from Amazon Glue DataBrew API
layout: schema
name: DescribeRecipeResponse
properties_list:
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: CreateDate
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: ProjectName
  type: object
- description: ''
  name: PublishedBy
  type: object
- description: ''
  name: PublishedDate
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Steps
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: RecipeVersion
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-describe-recipe-response-schema.json
slug: glue-databrew-describe-recipe-response
source_filename: glue-databrew-describe-recipe-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-recipe-response-schema.json\",\n  \"title\": \"DescribeRecipeResponse\",\n  \"description\": \"DescribeRecipeResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who created the recipe.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the recipe was created.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\
  \n        },\n        {\n          \"description\": \"The identifier (user name) of the user who last modified the recipe.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the recipe was last modified.\"\n        }\n      ]\n    },\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project associated with this recipe.\"\n        }\n      ]\n    },\n    \"PublishedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublishedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who last published the recipe.\"\n        }\n      ]\n    },\n    \"PublishedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\
  \n        },\n        {\n          \"description\": \"The date and time when the recipe was last published.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeDescription\"\n        },\n        {\n          \"description\": \"The description of the recipe.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The name of the recipe.\"\n        }\n      ]\n    },\n    \"Steps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeStepList\"\n        },\n        {\n          \"description\": \"One or more steps to be performed by the recipe. Each step consists of an action, and the conditions under which the action should succeed.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\
  \n        },\n        {\n          \"description\": \"Metadata tags associated with this project.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the recipe.\"\n        }\n      ]\n    },\n    \"RecipeVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeVersion\"\n        },\n        {\n          \"description\": \"The recipe version identifier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-recipe-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DescribeRecipeResponse
---
