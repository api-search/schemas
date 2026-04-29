---
description: CreateProjectRequest schema from Amazon Glue DataBrew API
layout: schema
name: CreateProjectRequest
properties_list:
- description: ''
  name: DatasetName
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RecipeName
  type: object
- description: ''
  name: Sample
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-create-project-request-schema.json
slug: glue-databrew-create-project-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-project-request-schema.json\",\n  \"title\": \"CreateProjectRequest\",\n  \"description\": \"CreateProjectRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\n        },\n        {\n          \"description\": \"The name of an existing dataset to associate this project with.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"A unique name for the new project. Valid characters are alphanumeric (A-Z, a-z, 0-9), hyphen (-), period (.), and space.\"\n        }\n      ]\n    },\n    \"RecipeName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n          \"description\": \"The name of an existing recipe to associate with the project.\"\n        }\n      ]\n    },\n    \"Sample\": {\n      \"$ref\": \"#/components/schemas/Sample\"\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role to be assumed for this request.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags to apply to this project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatasetName\",\n    \"Name\",\n    \"RecipeName\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-project-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CreateProjectRequest
---
