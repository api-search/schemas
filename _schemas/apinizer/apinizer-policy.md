---
description: Schema representing a security or governance policy in the Apinizer platform
layout: schema
name: Apinizer Policy
properties_list:
- description: Unique identifier of the policy
  name: id
  type: string
- description: Name of the policy
  name: name
  type: string
- description: Type of policy
  name: type
  type: string
- description: Policy-specific configuration parameters
  name: configuration
  type: object
provider_name: Apinizer
provider_slug: apinizer
schema_file: json-schema/apinizer-policy-schema.json
slug: apinizer-policy
tags:
- API Gateway
- API Management
- API Monitoring
- API Security
- Policies
title: Apinizer Policy
---
