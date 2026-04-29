---
description: Current data replication state and statistics for a source server
layout: schema
name: DataReplicationInfo
properties_list:
- description: Replication lag duration
  name: lagDuration
  type: string
- description: Date/time of the last snapshot
  name: lastSnapshotDateTime
  type: string
- description: List of replicated disks
  name: replicatedDisks
  type: array
- description: Current replication state
  name: dataReplicationState
  type: string
- description: dataReplicationInitiation
  name: dataReplicationInitiation
  type: string
- description: dataReplicationError
  name: dataReplicationError
  type: string
- description: Availability zone used for staging
  name: stagingAvailabilityZone
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-data-replication-info-schema.json
slug: application-migration-service-data-replication-info
source_filename: application-migration-service-data-replication-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-data-replication-info-schema.json\",\n  \"title\": \"DataReplicationInfo\",\n  \"description\": \"Current data replication state and statistics for a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lagDuration\": {\n      \"type\": \"string\",\n      \"description\": \"Replication lag duration\"\n    },\n    \"lastSnapshotDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time of the last snapshot\"\n    },\n    \"replicatedDisks\": {\n      \"type\": \"array\",\n      \"description\": \"List of replicated disks\"\n    },\n    \"dataReplicationState\": {\n      \"type\": \"string\",\n      \"description\": \"Current replication state\"\n    },\n    \"dataReplicationInitiation\": {\n      \"type\": \"string\",\n      \"description\": \"dataReplicationInitiation\"\
  \n    },\n    \"dataReplicationError\": {\n      \"type\": \"string\",\n      \"description\": \"dataReplicationError\"\n    },\n    \"stagingAvailabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"Availability zone used for staging\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-data-replication-info-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DataReplicationInfo
---
