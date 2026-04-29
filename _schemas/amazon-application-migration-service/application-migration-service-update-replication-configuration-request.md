---
description: Request to update replication configuration
layout: schema
name: UpdateReplicationConfigurationRequest
properties_list:
- description: Source server ID
  name: sourceServerID
  type: string
- description: Configuration name
  name: name
  type: string
- description: Subnet ID for staging area
  name: stagingAreaSubnetId
  type: string
- description: EC2 instance type for replication servers
  name: replicationServerInstanceType
  type: string
- description: Whether to use low bandwidth
  name: useLowBandwidthForReplication
  type: boolean
- description: Bandwidth throttling in Mbps
  name: bandwidthThrottling
  type: integer
- description: Data plane routing mode
  name: dataPlaneRouting
  type: string
- description: Whether to create public IP
  name: createPublicIP
  type: boolean
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-update-replication-configuration-request-schema.json
slug: application-migration-service-update-replication-configuration-request
source_filename: application-migration-service-update-replication-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-update-replication-configuration-request-schema.json\",\n  \"title\": \"UpdateReplicationConfigurationRequest\",\n  \"description\": \"Request to update replication configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name\"\n    },\n    \"stagingAreaSubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet ID for staging area\"\n    },\n    \"replicationServerInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"EC2 instance type for replication servers\"\n    },\n    \"useLowBandwidthForReplication\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether to use low bandwidth\"\n    },\n    \"bandwidthThrottling\": {\n      \"type\": \"integer\",\n      \"description\": \"Bandwidth throttling in Mbps\"\n    },\n    \"dataPlaneRouting\": {\n      \"type\": \"string\",\n      \"description\": \"Data plane routing mode\"\n    },\n    \"createPublicIP\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create public IP\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-update-replication-configuration-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: UpdateReplicationConfigurationRequest
---
