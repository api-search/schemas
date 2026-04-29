---
description: Request to update a launch configuration template
layout: schema
name: UpdateLaunchConfigurationTemplateRequest
properties_list:
- description: Template ID to update
  name: launchConfigurationTemplateID
  type: string
- description: launchDisposition
  name: launchDisposition
  type: string
- description: targetInstanceTypeRightSizingMethod
  name: targetInstanceTypeRightSizingMethod
  type: string
- description: copyPrivateIp
  name: copyPrivateIp
  type: boolean
- description: copyTags
  name: copyTags
  type: boolean
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-update-launch-configuration-template-request-schema.json
slug: application-migration-service-update-launch-configuration-template-request
source_filename: application-migration-service-update-launch-configuration-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-update-launch-configuration-template-request-schema.json\",\n  \"title\": \"UpdateLaunchConfigurationTemplateRequest\",\n  \"description\": \"Request to update a launch configuration template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"launchConfigurationTemplateID\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID to update\"\n    },\n    \"launchDisposition\": {\n      \"type\": \"string\",\n      \"description\": \"launchDisposition\"\n    },\n    \"targetInstanceTypeRightSizingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"targetInstanceTypeRightSizingMethod\"\n    },\n    \"copyPrivateIp\": {\n      \"type\": \"boolean\",\n      \"description\": \"copyPrivateIp\"\n    },\n    \"copyTags\": {\n      \"type\": \"boolean\",\n   \
  \   \"description\": \"copyTags\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-update-launch-configuration-template-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: UpdateLaunchConfigurationTemplateRequest
---
