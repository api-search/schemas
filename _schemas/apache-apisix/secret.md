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
