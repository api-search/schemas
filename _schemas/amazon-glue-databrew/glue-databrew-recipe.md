---
description: Represents one or more actions to be performed on a DataBrew dataset.
layout: schema
name: Recipe
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
  name: ResourceArn
  type: object
- description: ''
  name: Steps
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: RecipeVersion
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-recipe-schema.json
slug: glue-databrew-recipe
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-schema.json\",\n  \"title\": \"Recipe\",\n  \"description\": \"Represents one or more actions to be performed on a DataBrew dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who created the recipe.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the recipe was created.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who last modified the recipe.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The last modification date and time of the recipe.\"\n        }\n      ]\n    },\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project that the recipe is associated with.\"\n        }\n      ]\n    },\n    \"PublishedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublishedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who published the recipe.\"\n        }\n      ]\n    },\n    \"PublishedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time when the recipe was published.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeDescription\"\n        },\n        {\n          \"description\": \"The description of the recipe.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The unique name for the recipe.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the recipe.\"\n        }\n      ]\n    },\n    \"Steps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeStepList\"\n        },\n        {\n          \"description\"\
  : \"A list of steps that are defined by the recipe.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags that have been applied to the recipe.\"\n        }\n      ]\n    },\n    \"RecipeVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeVersion\"\n        },\n        {\n          \"description\": \"<p>The identifier for the version for the recipe. Must be one of the following:</p> <ul> <li> <p>Numeric version (<code>X.Y</code>) - <code>X</code> and <code>Y</code> stand for major and minor version numbers. The maximum length of each is 6 digits, and neither can be negative values. Both <code>X</code> and <code>Y</code> are required, and \\\"0.0\\\" isn't a valid version.</p> </li> <li> <p> <code>LATEST_WORKING</code> - the most recent valid version being developed in a DataBrew project.</p> </li> <li>\
  \ <p> <code>LATEST_PUBLISHED</code> - the most recent published version.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-recipe-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Recipe
---
