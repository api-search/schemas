---
description: An AppSumo software license purchased through the marketplace
layout: schema
name: License
properties_list:
- description: Unique license key for activation
  name: licenseKey
  type: string
- description: AppSumo product slug identifier
  name: productSlug
  type: string
- description: Current license status
  name: status
  type: string
- description: License tier (Tier 1, 2, 3, etc.)
  name: tier
  type: string
- description: When the license was activated
  name: activatedAt
  type: string
- description: AppSumo user who purchased the license
  name: userId
  type: string
- description: Purchaser email address
  name: email
  type: string
provider_name: AppSumo
provider_slug: appsumo
schema_file: json-schema/license-schema.json
slug: license
tags:
- Marketplace
- SaaS
- Software Deals
title: License
---
