---
description: Replication configuration for a source server
layout: schema
name: ReplicationConfiguration
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
- description: Whether to associate default security group
  name: associateDefaultSecurityGroup
  type: boolean
- description: Security group IDs for replication servers
  name: replicationServersSecurityGroupsIDs
  type: array
- description: EC2 instance type for replication servers
  name: replicationServerInstanceType
  type: string
- description: Whether to use low bandwidth for replication
  name: useLowBandwidthForReplication
  type: boolean
- description: Data plane routing mode
  name: dataPlaneRouting
  type: string
- description: Whether to create public IP for replication servers
  name: createPublicIP
  type: boolean
- description: Tags for staging area resources
  name: stagingAreaTags
  type: object
- description: Replicated disk configurations
  name: replicatedDisks
  type: array
- description: Bandwidth throttling in Mbps (0 for unlimited)
  name: bandwidthThrottling
  type: integer
- description: Default EBS volume type for large staging disks
  name: defaultLargeStagingDiskType
  type: string
- description: EBS encryption setting
  name: ebsEncryption
  type: string
- description: KMS key ARN for EBS encryption
  name: ebsEncryptionKeyArn
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-replication-configuration-schema.json
slug: application-migration-service-replication-configuration
source_filename: application-migration-service-replication-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-replication-configuration-schema.json\",\n  \"title\": \"ReplicationConfiguration\",\n  \"description\": \"Replication configuration for a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name\"\n    },\n    \"stagingAreaSubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet ID for staging area\"\n    },\n    \"associateDefaultSecurityGroup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to associate default security group\"\n    },\n    \"replicationServersSecurityGroupsIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Security\
  \ group IDs for replication servers\"\n    },\n    \"replicationServerInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"EC2 instance type for replication servers\"\n    },\n    \"useLowBandwidthForReplication\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use low bandwidth for replication\"\n    },\n    \"dataPlaneRouting\": {\n      \"type\": \"string\",\n      \"description\": \"Data plane routing mode\"\n    },\n    \"createPublicIP\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create public IP for replication servers\"\n    },\n    \"stagingAreaTags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags for staging area resources\"\n    },\n    \"replicatedDisks\": {\n      \"type\": \"array\",\n      \"description\": \"Replicated disk configurations\"\n    },\n    \"bandwidthThrottling\": {\n      \"type\": \"integer\",\n      \"description\": \"Bandwidth throttling in Mbps (0 for unlimited)\"\n  \
  \  },\n    \"defaultLargeStagingDiskType\": {\n      \"type\": \"string\",\n      \"description\": \"Default EBS volume type for large staging disks\"\n    },\n    \"ebsEncryption\": {\n      \"type\": \"string\",\n      \"description\": \"EBS encryption setting\"\n    },\n    \"ebsEncryptionKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"KMS key ARN for EBS encryption\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-replication-configuration-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: ReplicationConfiguration
---
