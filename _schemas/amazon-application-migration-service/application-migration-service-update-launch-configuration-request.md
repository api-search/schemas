---
description: Request to update launch configuration
layout: schema
name: UpdateLaunchConfigurationRequest
properties_list:
- description: Source server ID
  name: sourceServerID
  type: string
- description: Configuration name
  name: name
  type: string
- description: Launch disposition
  name: launchDisposition
  type: string
- description: Right-sizing method
  name: targetInstanceTypeRightSizingMethod
  type: string
- description: copyPrivateIp
  name: copyPrivateIp
  type: boolean
- description: copyTags
  name: copyTags
  type: boolean
- description: licensing
  name: licensing
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-update-launch-configuration-request-schema.json
slug: application-migration-service-update-launch-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-update-launch-configuration-request-schema.json\",\n  \"title\": \"UpdateLaunchConfigurationRequest\",\n  \"description\": \"Request to update launch configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name\"\n    },\n    \"launchDisposition\": {\n      \"type\": \"string\",\n      \"description\": \"Launch disposition\"\n    },\n    \"targetInstanceTypeRightSizingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Right-sizing method\"\n    },\n    \"copyPrivateIp\": {\n      \"type\": \"boolean\",\n      \"description\": \"copyPrivateIp\"\n    },\n    \"copyTags\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"copyTags\"\n    },\n    \"licensing\": {\n      \"type\": \"string\",\n      \"description\": \"licensing\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-update-launch-configuration-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: UpdateLaunchConfigurationRequest
---
