---
description: Information about an environment variable for a build project or a build.
layout: schema
name: EnvironmentVariable
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-environment-variable-schema.json
slug: amazon-codebuild-environment-variable
source_filename: amazon-codebuild-environment-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-variable-schema.json\",\n  \"title\": \"EnvironmentVariable\",\n  \"description\": \"Information about an environment variable for a build project or a build.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name or key of the environment variable.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The value of the environment variable.</p> <important> <p>We strongly discourage the use of <code>PLAINTEXT</code> environment variables to store sensitive values, especially Amazon\
  \ Web Services secret key IDs and secret access keys. <code>PLAINTEXT</code> environment variables can be displayed in plain text using the CodeBuild console and the CLI. For sensitive values, we recommend you use an environment variable of type <code>PARAMETER_STORE</code> or <code>SECRETS_MANAGER</code>. </p> </important>\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentVariableType\"\n        },\n        {\n          \"description\": \"<p>The type of environment variable. Valid values include:</p> <ul> <li> <p> <code>PARAMETER_STORE</code>: An environment variable stored in Systems Manager Parameter Store. To learn how to specify a parameter store environment variable, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html#build-spec.env.parameter-store\\\">env/parameter-store</a> in the <i>CodeBuild User Guide</i>.</p> </li> <li> <p> <code>PLAINTEXT</code>: An environment\
  \ variable in plain text format. This is the default value.</p> </li> <li> <p> <code>SECRETS_MANAGER</code>: An environment variable stored in Secrets Manager. To learn how to specify a secrets manager environment variable, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html#build-spec.env.secrets-manager\\\">env/secrets-manager</a> in the <i>CodeBuild User Guide</i>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-environment-variable-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: EnvironmentVariable
---
