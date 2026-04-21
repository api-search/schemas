---
description: PolicyRequest schema from Aqua Security API
layout: schema
name: PolicyRequest
properties_list:
- description: Policy name (unique)
  name: name
  type: string
- description: Policy description
  name: description
  type: string
- description: Block containers failing policy
  name: block_failed
  type: boolean
- description: Maximum CVSS score threshold
  name: maximum_score
  type: number
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-policy-request-schema.json
slug: aqua-security-api-policy-request
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: PolicyRequest
---
