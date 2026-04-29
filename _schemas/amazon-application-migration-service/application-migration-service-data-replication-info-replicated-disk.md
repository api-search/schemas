---
description: Replication status for an individual disk
layout: schema
name: DataReplicationInfoReplicatedDisk
properties_list:
- description: Device name of the disk
  name: deviceName
  type: string
- description: Total storage in bytes
  name: totalStorageBytes
  type: integer
- description: Amount of storage replicated in bytes
  name: replicatedStorageBytes
  type: integer
- description: Amount rescanned in bytes
  name: rescannedStorageBytes
  type: integer
- description: Amount backlogged in bytes
  name: backloggedStorageBytes
  type: integer
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-data-replication-info-replicated-disk-schema.json
slug: application-migration-service-data-replication-info-replicated-disk
source_filename: application-migration-service-data-replication-info-replicated-disk-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-data-replication-info-replicated-disk-schema.json\",\n  \"title\": \"DataReplicationInfoReplicatedDisk\",\n  \"description\": \"Replication status for an individual disk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Device name of the disk\"\n    },\n    \"totalStorageBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total storage in bytes\"\n    },\n    \"replicatedStorageBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount of storage replicated in bytes\"\n    },\n    \"rescannedStorageBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount rescanned in bytes\"\n    },\n    \"backloggedStorageBytes\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Amount backlogged in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-data-replication-info-replicated-disk-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DataReplicationInfoReplicatedDisk
---
