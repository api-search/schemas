---
description: ImageDetail schema from Aqua Security API
layout: schema
name: ImageDetail
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
- description: Operating system of the image
  name: os
  type: string
- description: Image size in bytes
  name: size
  type: integer
- description: Image creation timestamp
  name: created
  type: string
- description: Date the image was last scanned
  name: scan_date
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-image-detail-schema.json
slug: aqua-security-api-image-detail
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: ImageDetail
---
