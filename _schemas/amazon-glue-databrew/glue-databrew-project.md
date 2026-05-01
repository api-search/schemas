---
description: Represents all of the attributes of a DataBrew project.
layout: schema
name: Project
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: CreateDate
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: DatasetName
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RecipeName
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Sample
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: OpenedBy
  type: object
- description: ''
  name: OpenDate
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-project-schema.json
slug: glue-databrew-project
source_filename: glue-databrew-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"Represents all of the attributes of a DataBrew project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the project.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the project was created.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n \
  \       {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who crated the project.\"\n        }\n      ]\n    },\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\n        },\n        {\n          \"description\": \"The dataset that the project is to act upon.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The last modification date and time for the project.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who last modified the project.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\
  \n        },\n        {\n          \"description\": \"The unique name of a project.\"\n        }\n      ]\n    },\n    \"RecipeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The name of a recipe that will be developed during a project session.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the project.\"\n        }\n      ]\n    },\n    \"Sample\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sample\"\n        },\n        {\n          \"description\": \"The sample size and sampling type to apply to the data. If this parameter isn't specified, then the sample consists of the first 500 rows from the dataset.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags that have been applied to the project.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role that will be assumed for this project.\"\n        }\n      ]\n    },\n    \"OpenedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user that opened the project for use.\"\n        }\n      ]\n    },\n    \"OpenDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time when the project was opened.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n\
  \    \"RecipeName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-project-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Project
---
