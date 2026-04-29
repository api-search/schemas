---
description: ''
layout: schema
name: VxmlApplicationDetail
properties_list:
- description: ''
  name: applicationName
  type: string
- description: ''
  name: applicationType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: activeSessions
  type: integer
- description: ''
  name: deployedAt
  type: string
- description: ''
  name: description
  type: string
- description: Starting element of the call flow
  name: entryPoint
  type: string
- description: List of element names in the application
  name: elements
  type: array
- description: Path to the application media files
  name: mediaDirectory
  type: string
- description: Path to the application grammar files
  name: grammarDirectory
  type: string
- description: Application-level configuration parameters
  name: configParameters
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-vxml-application-detail-schema.json
slug: cisco-voice-portal-vxml-services-vxml-application-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VxmlApplicationDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"type\": \"string\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"activeSessions\": {\n      \"type\": \"integer\"\n    },\n    \"deployedAt\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"entryPoint\": {\n      \"type\": \"string\",\n      \"description\": \"Starting element of the call flow\"\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"description\": \"List of element names in the application\"\n    },\n    \"mediaDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the application media files\"\n    },\n    \"grammarDirectory\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"Path to the application grammar files\"\n    },\n    \"configParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Application-level configuration parameters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-vxml-application-detail-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: VxmlApplicationDetail
---
