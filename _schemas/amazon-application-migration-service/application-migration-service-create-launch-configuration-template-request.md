---
description: Request to create a launch configuration template
layout: schema
name: CreateLaunchConfigurationTemplateRequest
properties_list:
- description: Default launch disposition
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
- description: tags
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-create-launch-configuration-template-request-schema.json
slug: application-migration-service-create-launch-configuration-template-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-create-launch-configuration-template-request-schema.json\",\n  \"title\": \"CreateLaunchConfigurationTemplateRequest\",\n  \"description\": \"Request to create a launch configuration template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"launchDisposition\": {\n      \"type\": \"string\",\n      \"description\": \"Default launch disposition\"\n    },\n    \"targetInstanceTypeRightSizingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Right-sizing method\"\n    },\n    \"copyPrivateIp\": {\n      \"type\": \"boolean\",\n      \"description\": \"copyPrivateIp\"\n    },\n    \"copyTags\": {\n      \"type\": \"boolean\",\n      \"description\": \"copyTags\"\n    },\n    \"licensing\": {\n      \"type\": \"string\",\n      \"description\": \"licensing\"\n    },\n\
  \    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"tags\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-create-launch-configuration-template-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: CreateLaunchConfigurationTemplateRequest
---
