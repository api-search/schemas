---
description: Template for default replication configuration settings
layout: schema
name: ReplicationConfigurationTemplate
properties_list:
- description: Template ID
  name: replicationConfigurationTemplateID
  type: string
- description: ARN of the template
  name: arn
  type: string
- description: Subnet ID for staging area
  name: stagingAreaSubnetId
  type: string
- description: Whether to associate default security group
  name: associateDefaultSecurityGroup
  type: boolean
- description: Security group IDs
  name: replicationServersSecurityGroupsIDs
  type: array
- description: EC2 instance type for replication servers
  name: replicationServerInstanceType
  type: string
- description: Whether to use low bandwidth
  name: useLowBandwidthForReplication
  type: boolean
- description: Data plane routing mode
  name: dataPlaneRouting
  type: string
- description: Whether to create public IP
  name: createPublicIP
  type: boolean
- description: Tags for staging resources
  name: stagingAreaTags
  type: object
- description: Bandwidth throttling in Mbps
  name: bandwidthThrottling
  type: integer
- description: Default disk type for large disks
  name: defaultLargeStagingDiskType
  type: string
- description: EBS encryption setting
  name: ebsEncryption
  type: string
- description: Tags on the template
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-replication-configuration-template-schema.json
slug: application-migration-service-replication-configuration-template
source_filename: application-migration-service-replication-configuration-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-replication-configuration-template-schema.json\",\n  \"title\": \"ReplicationConfigurationTemplate\",\n  \"description\": \"Template for default replication configuration settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"replicationConfigurationTemplateID\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the template\"\n    },\n    \"stagingAreaSubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet ID for staging area\"\n    },\n    \"associateDefaultSecurityGroup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to associate default security group\"\n    },\n    \"replicationServersSecurityGroupsIDs\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"Security group IDs\"\n    },\n    \"replicationServerInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"EC2 instance type for replication servers\"\n    },\n    \"useLowBandwidthForReplication\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use low bandwidth\"\n    },\n    \"dataPlaneRouting\": {\n      \"type\": \"string\",\n      \"description\": \"Data plane routing mode\"\n    },\n    \"createPublicIP\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create public IP\"\n    },\n    \"stagingAreaTags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags for staging resources\"\n    },\n    \"bandwidthThrottling\": {\n      \"type\": \"integer\",\n      \"description\": \"Bandwidth throttling in Mbps\"\n    },\n    \"defaultLargeStagingDiskType\": {\n      \"type\": \"string\",\n      \"description\": \"Default disk type for large disks\"\n    },\n    \"ebsEncryption\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"EBS encryption setting\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the template\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-replication-configuration-template-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ReplicationConfigurationTemplate
---
