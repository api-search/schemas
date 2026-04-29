---
description: Template for default launch configuration settings
layout: schema
name: LaunchConfigurationTemplate
properties_list:
- description: Template ID
  name: launchConfigurationTemplateID
  type: string
- description: ARN of the template
  name: arn
  type: string
- description: Default launch disposition
  name: launchDisposition
  type: string
- description: Right-sizing method
  name: targetInstanceTypeRightSizingMethod
  type: string
- description: Whether to copy private IP
  name: copyPrivateIp
  type: boolean
- description: Whether to copy tags
  name: copyTags
  type: boolean
- description: licensing
  name: licensing
  type: string
- description: Boot mode
  name: bootMode
  type: string
- description: Tags on the template
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-launch-configuration-template-schema.json
slug: application-migration-service-launch-configuration-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-launch-configuration-template-schema.json\",\n  \"title\": \"LaunchConfigurationTemplate\",\n  \"description\": \"Template for default launch configuration settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"launchConfigurationTemplateID\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the template\"\n    },\n    \"launchDisposition\": {\n      \"type\": \"string\",\n      \"description\": \"Default launch disposition\"\n    },\n    \"targetInstanceTypeRightSizingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Right-sizing method\"\n    },\n    \"copyPrivateIp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to copy private\
  \ IP\"\n    },\n    \"copyTags\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to copy tags\"\n    },\n    \"licensing\": {\n      \"type\": \"string\",\n      \"description\": \"licensing\"\n    },\n    \"bootMode\": {\n      \"type\": \"string\",\n      \"description\": \"Boot mode\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the template\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-launch-configuration-template-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: LaunchConfigurationTemplate
---
