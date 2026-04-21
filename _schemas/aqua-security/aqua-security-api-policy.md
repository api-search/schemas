---
description: Policy schema from Aqua Security API
layout: schema
name: Policy
properties_list:
- description: Policy name
  name: name
  type: string
- description: Policy description
  name: description
  type: string
- description: Whether to block containers that fail policy evaluation
  name: block_failed
  type: boolean
- description: Maximum CVSS score allowed (0-10)
  name: maximum_score
  type: number
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-policy-schema.json
slug: aqua-security-api-policy
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: Policy
---
