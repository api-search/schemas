---
description: Represents an Amazon Web Services session credentials object. These credentials are temporary credentials that are issued by Amazon Web Services Secure Token Service (STS). They can be used to access input and output artifacts in the S3 bucket used to store artifact for the pipeline in CodePipeline.
layout: schema
name: AWSSessionCredentials
properties_list:
- description: ''
  name: accessKeyId
  type: object
- description: ''
  name: secretAccessKey
  type: object
- description: ''
  name: sessionToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-aws-session-credentials-schema.json
slug: amazon-codepipeline-aws-session-credentials
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-aws-session-credentials-schema.json\",\n  \"title\": \"AWSSessionCredentials\",\n  \"description\": \"Represents an Amazon Web Services session credentials object. These credentials are temporary credentials that are issued by Amazon Web Services Secure Token Service (STS). They can be used to access input and output artifacts in the S3 bucket used to store artifact for the pipeline in CodePipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessKeyId\"\n        },\n        {\n          \"description\": \"The access key for the session.\"\n        }\n      ]\n    },\n    \"secretAccessKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretAccessKey\"\
  \n        },\n        {\n          \"description\": \"The secret access key for the session.\"\n        }\n      ]\n    },\n    \"sessionToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionToken\"\n        },\n        {\n          \"description\": \"The token for the session.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessKeyId\",\n    \"secretAccessKey\",\n    \"sessionToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-aws-session-credentials-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: AWSSessionCredentials
---
