---
description: Image schema from Aqua Security API
layout: schema
name: Image
properties_list:
- description: Name of the container registry
  name: registry
  type: string
- description: Image repository name
  name: name
  type: string
- description: Image tag
  name: tag
  type: string
- description: Image content digest (SHA256)
  name: digest
  type: string
- description: Current scan status
  name: scan_status
  type: string
- description: ''
  name: vulnerabilities
  type: object
- description: Whether the image is blocked by policy
  name: disallowed
  type: boolean
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-image-schema.json
slug: aqua-security-api-image
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: Image
---
