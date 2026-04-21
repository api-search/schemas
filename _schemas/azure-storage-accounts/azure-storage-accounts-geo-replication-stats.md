---
description: Statistics related to replication for storage account's Blob, Table, Queue and File services. It is only available when geo-redundant replication is enabled for the storage account.
layout: schema
name: GeoReplicationStats
properties_list:
- description: A boolean flag which indicates whether or not account failover is supported for the account.
  name: canFailover
  type: boolean
- description: All primary writes preceding this UTC date/time value are guaranteed to be available for read operations. Primary writes following this point in time may or may not be available for reads. Element may
  name: lastSyncTime
  type: string
- description: 'The status of the secondary location. Possible values are: - Live: Indicates that the secondary location is active and operational. - Bootstrap: Indicates initial synchronization from the primary loca'
  name: status
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-geo-replication-stats-schema.json
slug: azure-storage-accounts-geo-replication-stats
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: GeoReplicationStats
---
