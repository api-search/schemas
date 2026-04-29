---
description: Launch configuration for a source server
layout: schema
name: LaunchConfiguration
properties_list:
- description: Source server ID
  name: sourceServerID
  type: string
- description: Configuration name
  name: name
  type: string
- description: EC2 launch template ID
  name: ec2LaunchTemplateID
  type: string
- description: Launch disposition for the instance
  name: launchDisposition
  type: string
- description: Right-sizing method for target instance type
  name: targetInstanceTypeRightSizingMethod
  type: string
- description: Whether to copy source server private IP to target
  name: copyPrivateIp
  type: boolean
- description: Whether to copy source server tags to target instance
  name: copyTags
  type: boolean
- description: licensing
  name: licensing
  type: string
- description: Boot mode for the target instance
  name: bootMode
  type: string
- description: postLaunchActions
  name: postLaunchActions
  type: string
- description: Whether to enable MAP auto-tagging
  name: enableMapAutoTagging
  type: boolean
- description: MAP auto-tagging MPE ID
  name: mapAutoTaggingMpeID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-launch-configuration-schema.json
slug: application-migration-service-launch-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-launch-configuration-schema.json\",\n  \"title\": \"LaunchConfiguration\",\n  \"description\": \"Launch configuration for a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name\"\n    },\n    \"ec2LaunchTemplateID\": {\n      \"type\": \"string\",\n      \"description\": \"EC2 launch template ID\"\n    },\n    \"launchDisposition\": {\n      \"type\": \"string\",\n      \"description\": \"Launch disposition for the instance\"\n    },\n    \"targetInstanceTypeRightSizingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Right-sizing method for target instance type\"\
  \n    },\n    \"copyPrivateIp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to copy source server private IP to target\"\n    },\n    \"copyTags\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to copy source server tags to target instance\"\n    },\n    \"licensing\": {\n      \"type\": \"string\",\n      \"description\": \"licensing\"\n    },\n    \"bootMode\": {\n      \"type\": \"string\",\n      \"description\": \"Boot mode for the target instance\"\n    },\n    \"postLaunchActions\": {\n      \"type\": \"string\",\n      \"description\": \"postLaunchActions\"\n    },\n    \"enableMapAutoTagging\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable MAP auto-tagging\"\n    },\n    \"mapAutoTaggingMpeID\": {\n      \"type\": \"string\",\n      \"description\": \"MAP auto-tagging MPE ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-launch-configuration-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: LaunchConfiguration
---
