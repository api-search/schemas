---
description: Lease Container request schema.
layout: schema
name: LeaseContainerRequest
properties_list:
- description: Specifies the lease action. Can be one of the available actions.
  name: action
  type: string
- description: Optional. For a break action, proposed duration the lease should continue before it is broken, in seconds, between 0 and 60.
  name: breakPeriod
  type: integer
- description: Required for acquire. Specifies the duration of the lease, in seconds, or negative one (-1) for a lease that never expires.
  name: leaseDuration
  type: integer
- description: Identifies the lease. Can be specified in any valid GUID string format.
  name: leaseId
  type: string
- description: Optional for acquire, required for change. Proposed lease ID, in a GUID string format.
  name: proposedLeaseId
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-lease-container-request-schema.json
slug: azure-storage-account-lease-container-request
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: LeaseContainerRequest
---
