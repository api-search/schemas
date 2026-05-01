---
description: Request to update a replication configuration template
layout: schema
name: UpdateReplicationConfigurationTemplateRequest
properties_list:
- description: Template ID to update
  name: replicationConfigurationTemplateID
  type: string
- description: stagingAreaSubnetId
  name: stagingAreaSubnetId
  type: string
- description: associateDefaultSecurityGroup
  name: associateDefaultSecurityGroup
  type: boolean
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
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-update-replication-configuration-template-request-schema.json
slug: application-migration-service-update-replication-configuration-template-request
source_filename: application-migration-service-update-replication-configuration-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-update-replication-configuration-template-request-schema.json\",\n  \"title\": \"UpdateReplicationConfigurationTemplateRequest\",\n  \"description\": \"Request to update a replication configuration template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"replicationConfigurationTemplateID\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID to update\"\n    },\n    \"stagingAreaSubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"stagingAreaSubnetId\"\n    },\n    \"associateDefaultSecurityGroup\": {\n      \"type\": \"boolean\",\n      \"description\": \"associateDefaultSecurityGroup\"\n    },\n    \"replicationServerInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"replicationServerInstanceType\"\n    },\n    \"useLowBandwidthForReplication\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"useLowBandwidthForReplication\"\n    },\n    \"dataPlaneRouting\": {\n      \"type\": \"string\",\n      \"description\": \"dataPlaneRouting\"\n    },\n    \"createPublicIP\": {\n      \"type\": \"boolean\",\n      \"description\": \"createPublicIP\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-update-replication-configuration-template-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: UpdateReplicationConfigurationTemplateRequest
---
