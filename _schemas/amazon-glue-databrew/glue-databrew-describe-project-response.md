---
description: DescribeProjectResponse schema from Amazon Glue DataBrew API
layout: schema
name: DescribeProjectResponse
properties_list:
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
  name: RoleArn
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: SessionStatus
  type: object
- description: ''
  name: OpenedBy
  type: object
- description: ''
  name: OpenDate
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-describe-project-response-schema.json
slug: glue-databrew-describe-project-response
source_filename: glue-databrew-describe-project-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-project-response-schema.json\",\n  \"title\": \"DescribeProjectResponse\",\n  \"description\": \"DescribeProjectResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the project was created.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who created the project.\"\n        }\n      ]\n    },\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\
  \n        },\n        {\n          \"description\": \"The dataset associated with the project.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the project was last modified.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who last modified the project.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project.\"\n        }\n      ]\n    },\n    \"RecipeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeName\"\n        },\n        {\n     \
  \     \"description\": \"The recipe associated with this job.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the project.\"\n        }\n      ]\n    },\n    \"Sample\": {\n      \"$ref\": \"#/components/schemas/Sample\"\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the Identity and Access Management (IAM) role to be assumed when DataBrew runs the job.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags associated with this project.\"\n        }\n      ]\n    },\n    \"SessionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionStatus\"\
  \n        },\n        {\n          \"description\": \"<p>Describes the current state of the session:</p> <ul> <li> <p> <code>PROVISIONING</code> - allocating resources for the session.</p> </li> <li> <p> <code>INITIALIZING</code> - getting the session ready for first use.</p> </li> <li> <p> <code>ASSIGNED</code> - the session is ready for use.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"OpenedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user that opened the project for use. \"\n        }\n      ]\n    },\n    \"OpenDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time when the project was opened. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-project-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DescribeProjectResponse
---
