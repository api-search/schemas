---
description: Request body for updating an existing CloudHub application
layout: schema
name: ApplicationUpdate
properties_list:
- description: New Mule runtime version
  name: muleVersion
  type: object
- description: Updated application properties
  name: properties
  type: object
- description: Enable or disable automatic restart
  name: monitoringAutoRestart
  type: boolean
- description: Target CloudHub region
  name: region
  type: string
- description: Enable or disable static IPs
  name: staticIPsEnabled
  type: boolean
- description: Enable or disable next-generation logging
  name: loggingNgEnabled
  type: boolean
- description: Enable or disable persistent queues
  name: persistentQueues
  type: boolean
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-application-update-schema.json
slug: mulesoft-anypoint-platform-application-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an existing CloudHub application\",\n  \"properties\": {\n    \"muleVersion\": {\n      \"type\": \"object\",\n      \"description\": \"New Mule runtime version\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Updated application properties\"\n    },\n    \"monitoringAutoRestart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable or disable automatic restart\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Target CloudHub region\"\n    },\n    \"staticIPsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable or disable static IPs\"\n    },\n    \"loggingNgEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable or disable next-generation logging\"\n    },\n    \"persistentQueues\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Enable or disable persistent queues\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-application-update-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: ApplicationUpdate
---
