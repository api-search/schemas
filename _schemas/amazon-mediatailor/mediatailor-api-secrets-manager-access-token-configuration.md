---
description: AWS Secrets Manager access token configuration parameters. For information about Secrets Manager access token authentication, see <a href="https://docs.aws.amazon.com/mediatailor/latest/ug/channel-assembly-access-configuration-access-token.html">Working with AWS Secrets Manager access token authentication</a>.
layout: schema
name: SecretsManagerAccessTokenConfiguration
properties_list:
- description: ''
  name: HeaderName
  type: object
- description: ''
  name: SecretArn
  type: object
- description: ''
  name: SecretStringKey
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-secrets-manager-access-token-configuration-schema.json
slug: mediatailor-api-secrets-manager-access-token-configuration
source_filename: mediatailor-api-secrets-manager-access-token-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-secrets-manager-access-token-configuration-schema.json\",\n  \"title\": \"SecretsManagerAccessTokenConfiguration\",\n  \"description\": \"AWS Secrets Manager access token configuration parameters. For information about Secrets Manager access token authentication, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/channel-assembly-access-configuration-access-token.html\\\">Working with AWS Secrets Manager access token authentication</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HeaderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the HTTP header used to supply the access token in requests to the source location.\"\n        }\n      ]\n    },\n\
  \    \"SecretArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Secrets Manager secret that contains the access token.\"\n        }\n      ]\n    },\n    \"SecretStringKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The AWS Secrets Manager <a href=\\\"https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_CreateSecret.html#SecretsManager-CreateSecret-request-SecretString.html\\\">SecretString</a> key associated with the access token. MediaTailor uses the key to look up SecretString key and value pair containing the access token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-secrets-manager-access-token-configuration-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SecretsManagerAccessTokenConfiguration
---
