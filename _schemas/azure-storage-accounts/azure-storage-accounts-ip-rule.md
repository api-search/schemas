---
description: IP rule with specific IP or IP range in CIDR format.
layout: schema
name: IPRule
properties_list:
- description: The action of IP ACL rule.
  name: action
  type: string
- description: Specifies the IP or IP range in CIDR format. Only IPV4 address is allowed.
  name: value
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-ip-rule-schema.json
slug: azure-storage-accounts-ip-rule
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: IPRule
---
