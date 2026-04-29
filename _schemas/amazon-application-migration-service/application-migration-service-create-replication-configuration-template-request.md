---
description: Request to create a replication configuration template
layout: schema
name: CreateReplicationConfigurationTemplateRequest
properties_list:
- description: Subnet ID
  name: stagingAreaSubnetId
  type: string
- description: Associate default security group
  name: associateDefaultSecurityGroup
  type: boolean
- description: replicationServersSecurityGroupsIDs
  name: replicationServersSecurityGroupsIDs
  type: array
- description: replicationServerInstanceType
  name: replicationServerInstanceType
  type: string
- description: useLowBandwidthForReplication
  name: useLowBandwidthForReplication
  type: boolean
- description: dataPlaneRouting
  name: dataPlaneRouting
  type: string
- description: createPublicIP
  name: createPublicIP
  type: boolean
- description: stagingAreaTags
  name: stagingAreaTags
  type: object
- description: defaultLargeStagingDiskType
  name: defaultLargeStagingDiskType
  type: string
- description: ebsEncryption
  name: ebsEncryption
  type: string
- description: bandwidthThrottling
  name: bandwidthThrottling
  type: integer
- description: tags
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-create-replication-configuration-template-request-schema.json
slug: application-migration-service-create-replication-configuration-template-request
source_filename: application-migration-service-create-replication-configuration-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-create-replication-configuration-template-request-schema.json\",\n  \"title\": \"CreateReplicationConfigurationTemplateRequest\",\n  \"description\": \"Request to create a replication configuration template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stagingAreaSubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet ID\"\n    },\n    \"associateDefaultSecurityGroup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Associate default security group\"\n    },\n    \"replicationServersSecurityGroupsIDs\": {\n      \"type\": \"array\",\n      \"description\": \"replicationServersSecurityGroupsIDs\"\n    },\n    \"replicationServerInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"replicationServerInstanceType\"\n    },\n   \
  \ \"useLowBandwidthForReplication\": {\n      \"type\": \"boolean\",\n      \"description\": \"useLowBandwidthForReplication\"\n    },\n    \"dataPlaneRouting\": {\n      \"type\": \"string\",\n      \"description\": \"dataPlaneRouting\"\n    },\n    \"createPublicIP\": {\n      \"type\": \"boolean\",\n      \"description\": \"createPublicIP\"\n    },\n    \"stagingAreaTags\": {\n      \"type\": \"object\",\n      \"description\": \"stagingAreaTags\"\n    },\n    \"defaultLargeStagingDiskType\": {\n      \"type\": \"string\",\n      \"description\": \"defaultLargeStagingDiskType\"\n    },\n    \"ebsEncryption\": {\n      \"type\": \"string\",\n      \"description\": \"ebsEncryption\"\n    },\n    \"bandwidthThrottling\": {\n      \"type\": \"integer\",\n      \"description\": \"bandwidthThrottling\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"tags\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-create-replication-configuration-template-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: CreateReplicationConfigurationTemplateRequest
---
