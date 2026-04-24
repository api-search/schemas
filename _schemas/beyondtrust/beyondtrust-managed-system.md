---
description: A system registered in BeyondTrust Password Safe.
layout: schema
name: ManagedSystem
properties_list:
- description: Unique identifier of the managed system.
  name: ManagedSystemID
  type: integer
- description: Name of the system.
  name: SystemName
  type: string
- description: IP address of the system.
  name: IPAddress
  type: string
- description: Operating system platform.
  name: Platform
  type: string
- description: Network hostname or FQDN.
  name: NetworkAddress
  type: string
- description: Contact email for this system.
  name: ContactEmail
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-managed-system-schema.json
slug: beyondtrust-managed-system
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: ManagedSystem
---
