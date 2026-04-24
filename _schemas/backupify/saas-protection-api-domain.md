---
description: A SaaS customer domain with backup subscription information
layout: schema
name: Domain
properties_list:
- description: Unique SaaS customer identifier
  name: saasCustomerId
  type: string
- description: External subscription identifier for seat management
  name: externalSubscriptionId
  type: string
- description: The domain name (e.g., company.onmicrosoft.com)
  name: domain
  type: string
- description: Domain backup status
  name: status
  type: string
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-domain-schema.json
slug: saas-protection-api-domain
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: Domain
---
