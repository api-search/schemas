---
description: A privileged account managed by BeyondTrust Password Safe.
layout: schema
name: ManagedAccount
properties_list:
- description: Unique identifier of the managed account.
  name: AccountID
  type: integer
- description: Name of the privileged account.
  name: AccountName
  type: string
- description: ID of the managed system.
  name: SystemID
  type: integer
- description: Name of the system containing this account.
  name: SystemName
  type: string
- description: Domain name for domain accounts.
  name: DomainName
  type: string
- description: Type of account.
  name: AccountType
  type: string
- description: When the password was last changed.
  name: LastChangeDate
  type: string
- description: Whether password fallback is enabled.
  name: PasswordFallbackFlag
  type: boolean
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-managed-account-schema.json
slug: beyondtrust-managed-account
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: ManagedAccount
---
