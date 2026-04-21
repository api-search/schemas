---
description: Container schema from Aqua Security API
layout: schema
name: Container
properties_list:
- description: Container ID
  name: container_id
  type: string
- description: Container name
  name: name
  type: string
- description: Image name and tag
  name: image
  type: string
- description: Container runtime status
  name: status
  type: string
- description: Applied security policy name
  name: policy
  type: string
- description: Host running the container
  name: host
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-container-schema.json
slug: aqua-security-api-container
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: Container
---
