---
description: UpdateJobFromSourceControlRequest schema from Amazon Glue API
layout: schema
name: UpdateJobFromSourceControlRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: Provider
  type: object
- description: ''
  name: RepositoryName
  type: object
- description: ''
  name: RepositoryOwner
  type: object
- description: ''
  name: BranchName
  type: object
- description: ''
  name: Folder
  type: object
- description: ''
  name: CommitId
  type: object
- description: ''
  name: AuthStrategy
  type: object
- description: ''
  name: AuthToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-job-from-source-control-request-schema.json
slug: glue-update-job-from-source-control-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-job-from-source-control-request-schema.json\",\n  \"title\": \"UpdateJobFromSourceControlRequest\",\n  \"description\": \"UpdateJobFromSourceControlRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the Glue job to be synchronized to or from the remote repository.\"\n        }\n      ]\n    },\n    \"Provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceControlProvider\"\n        },\n        {\n          \"description\": \"The provider for the remote repository.\"\n        }\n      ]\n    },\n    \"RepositoryName\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the remote repository that contains the job artifacts.\"\n        }\n      ]\n    },\n    \"RepositoryOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The owner of the remote repository that contains the job artifacts.\"\n        }\n      ]\n    },\n    \"BranchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"An optional branch in the remote repository.\"\n        }\n      ]\n    },\n    \"Folder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"An optional folder in the remote repository.\"\n        }\n      ]\n    },\n    \"CommitId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/CommitIdString\"\n        },\n        {\n          \"description\": \"A commit ID for a commit in the remote repository.\"\n        }\n      ]\n    },\n    \"AuthStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceControlAuthStrategy\"\n        },\n        {\n          \"description\": \"The type of authentication, which can be an authentication token stored in Amazon Web Services Secrets Manager, or a personal access token.\"\n        }\n      ]\n    },\n    \"AuthToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthTokenString\"\n        },\n        {\n          \"description\": \"The value of the authorization token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-job-from-source-control-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateJobFromSourceControlRequest
---
