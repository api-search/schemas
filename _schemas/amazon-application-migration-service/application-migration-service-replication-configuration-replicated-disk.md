---
description: Replication configuration for an individual disk
layout: schema
name: ReplicationConfigurationReplicatedDisk
properties_list:
- description: Device name
  name: deviceName
  type: string
- description: Whether this is the boot disk
  name: isBootDisk
  type: boolean
- description: EBS volume type for staging
  name: stagingDiskType
  type: string
- description: IOPS for the staging disk
  name: iops
  type: integer
- description: Throughput for the staging disk in MB/s
  name: throughput
  type: integer
- description: Optimized staging disk type recommendation
  name: optimizedStagingDiskType
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-replication-configuration-replicated-disk-schema.json
slug: application-migration-service-replication-configuration-replicated-disk
source_filename: application-migration-service-replication-configuration-replicated-disk-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-replication-configuration-replicated-disk-schema.json\",\n  \"title\": \"ReplicationConfigurationReplicatedDisk\",\n  \"description\": \"Replication configuration for an individual disk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Device name\"\n    },\n    \"isBootDisk\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the boot disk\"\n    },\n    \"stagingDiskType\": {\n      \"type\": \"string\",\n      \"description\": \"EBS volume type for staging\"\n    },\n    \"iops\": {\n      \"type\": \"integer\",\n      \"description\": \"IOPS for the staging disk\"\n    },\n    \"throughput\": {\n      \"type\": \"integer\",\n      \"description\": \"Throughput for the staging disk\
  \ in MB/s\"\n    },\n    \"optimizedStagingDiskType\": {\n      \"type\": \"string\",\n      \"description\": \"Optimized staging disk type recommendation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-replication-configuration-replicated-disk-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ReplicationConfigurationReplicatedDisk
---
