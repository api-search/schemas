---
description: A Secret resource manages integration with external secret managers such as HashiCorp Vault or AWS Secrets Manager.
layout: schema
name: Apache APISIX Secret
properties_list:
- description: URI of the secret manager endpoint.
  name: uri
  type: string
- description: Path prefix in the secret manager.
  name: prefix
  type: string
- description: Authentication token for the secret manager.
  name: token
  type: string
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/secret.json
slug: secret
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/secret.json\",\n  \"title\": \"Apache APISIX Secret\",\n  \"description\": \"A Secret resource manages integration with external secret managers such as HashiCorp Vault or AWS Secrets Manager.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the secret manager endpoint.\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Path prefix in the secret manager.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication token for the secret manager.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/secret.json
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Secret
---
