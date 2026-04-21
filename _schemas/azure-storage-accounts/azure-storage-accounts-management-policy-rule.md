---
description: An object that wraps the Lifecycle rule. Each rule is uniquely defined by name.
layout: schema
name: ManagementPolicyRule
properties_list:
- description: An object that defines the Lifecycle rule.
  name: definition
  type: object
- description: Rule is enabled if set to true.
  name: enabled
  type: boolean
- description: A rule name can contain any combination of alpha numeric characters. Rule name is case-sensitive. It must be unique within a policy.
  name: name
  type: string
- description: The valid value is Lifecycle
  name: type
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-management-policy-rule-schema.json
slug: azure-storage-accounts-management-policy-rule
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ManagementPolicyRule
---
