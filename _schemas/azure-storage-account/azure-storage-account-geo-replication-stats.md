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
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-geo-replication-stats-schema.json
slug: azure-storage-account-geo-replication-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-geo-replication-stats-schema.json\",\n  \"title\": \"GeoReplicationStats\",\n  \"description\": \"Statistics related to replication for storage account's Blob, Table, Queue and File services. It is only available when geo-redundant replication is enabled for the storage account.\",\n  \"properties\": {\n    \"canFailover\": {\n      \"description\": \"A boolean flag which indicates whether or not account failover is supported for the account.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"lastSyncTime\": {\n      \"description\": \"All primary writes preceding this UTC date/time value are guaranteed to be available for read operations. Primary writes following this point in time may or may not be available for reads. Element may be default value if\
  \ value of LastSyncTime is not available, this can happen if secondary is offline or we are in bootstrap.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the secondary location. Possible values are: - Live: Indicates that the secondary location is active and operational. - Bootstrap: Indicates initial synchronization from the primary location to the secondary location is in progress.This typically occurs when replication is first enabled. - Unavailable: Indicates that the secondary location is temporarily unavailable.\",\n      \"enum\": [\n        \"Live\",\n        \"Bootstrap\",\n        \"Unavailable\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"GeoReplicationStatus\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-geo-replication-stats-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: GeoReplicationStats
---
