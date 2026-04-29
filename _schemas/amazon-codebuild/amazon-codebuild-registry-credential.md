---
description: '<p> Information about credentials that provide access to a private Docker registry. When this is set: </p> <ul> <li> <p> <code>imagePullCredentialsType</code> must be set to <code>SERVICE_ROLE</code>. </p> </li> <li> <p> images cannot be curated or an Amazon ECR image.</p> </li> </ul> <p> For more information, see <a href="https://docs.aws.amazon.com/codebuild/latest/userguide/sample-private-registry.html">Private Registry with Secrets Manager Sample for CodeBuild</a>. </p>'
layout: schema
name: RegistryCredential
properties_list:
- description: ''
  name: credential
  type: object
- description: ''
  name: credentialProvider
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-registry-credential-schema.json
slug: amazon-codebuild-registry-credential
source_filename: amazon-codebuild-registry-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-registry-credential-schema.json\",\n  \"title\": \"RegistryCredential\",\n  \"description\": \"<p> Information about credentials that provide access to a private Docker registry. When this is set: </p> <ul> <li> <p> <code>imagePullCredentialsType</code> must be set to <code>SERVICE_ROLE</code>. </p> </li> <li> <p> images cannot be curated or an Amazon ECR image.</p> </li> </ul> <p> For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/sample-private-registry.html\\\">Private Registry with Secrets Manager Sample for CodeBuild</a>. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"credential\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\":\
  \ \"<p> The Amazon Resource Name (ARN) or name of credentials created using Secrets Manager. </p> <note> <p> The <code>credential</code> can use the name of the credentials only if they exist in your current Amazon Web Services Region. </p> </note>\"\n        }\n      ]\n    },\n    \"credentialProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CredentialProviderType\"\n        },\n        {\n          \"description\": \" The service that created the credentials to access a private Docker registry. The valid value, SECRETS_MANAGER, is for Secrets Manager. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"credential\",\n    \"credentialProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-registry-credential-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: RegistryCredential
---
