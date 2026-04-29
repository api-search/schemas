---
description: ''
layout: schema
name: CallDetailRecord
properties_list:
- description: Globally unique call identifier
  name: callGuid
  type: string
- description: Call start timestamp
  name: callStartTime
  type: string
- description: Call end timestamp
  name: callEndTime
  type: string
- description: Caller ANI (Automatic Number Identification)
  name: callingNumber
  type: string
- description: Called DNIS (Dialed Number Identification Service)
  name: calledNumber
  type: string
- description: Final call outcome
  name: callResult
  type: string
- description: Total call duration in seconds
  name: callDuration
  type: integer
- description: Duration of self-service (IVR) portion in seconds
  name: selfServiceDuration
  type: integer
- description: Duration in queue in seconds
  name: queueDuration
  type: integer
- description: VXML application that handled the call
  name: applicationName
  type: string
- description: Call Server that processed the call
  name: callServerHostname
  type: string
- description: VXML Server that executed the application
  name: vxmlServerHostname
  type: string
- description: SIP Call-ID header value
  name: sipCallId
  type: string
- description: ICM/UCCE call key for correlation
  name: icmCallKey
  type: string
- description: Expanded Call Context (ECC) variables
  name: eccVariables
  type: object
- description: Transfer destination number if the call was transferred
  name: transferDestination
  type: string
- description: Error code if the call ended in error
  name: errorCode
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-call-detail-record-schema.json
slug: cisco-voice-portal-reporting-call-detail-record
source_filename: cisco-voice-portal-reporting-call-detail-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallDetailRecord\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callGuid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique call identifier\"\n    },\n    \"callStartTime\": {\n      \"type\": \"string\",\n      \"description\": \"Call start timestamp\"\n    },\n    \"callEndTime\": {\n      \"type\": \"string\",\n      \"description\": \"Call end timestamp\"\n    },\n    \"callingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Caller ANI (Automatic Number Identification)\"\n    },\n    \"calledNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Called DNIS (Dialed Number Identification Service)\"\n    },\n    \"callResult\": {\n      \"type\": \"string\",\n      \"description\": \"Final call outcome\"\n    },\n    \"callDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Total call duration in seconds\"\n\
  \    },\n    \"selfServiceDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of self-service (IVR) portion in seconds\"\n    },\n    \"queueDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration in queue in seconds\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"VXML application that handled the call\"\n    },\n    \"callServerHostname\": {\n      \"type\": \"string\",\n      \"description\": \"Call Server that processed the call\"\n    },\n    \"vxmlServerHostname\": {\n      \"type\": \"string\",\n      \"description\": \"VXML Server that executed the application\"\n    },\n    \"sipCallId\": {\n      \"type\": \"string\",\n      \"description\": \"SIP Call-ID header value\"\n    },\n    \"icmCallKey\": {\n      \"type\": \"string\",\n      \"description\": \"ICM/UCCE call key for correlation\"\n    },\n    \"eccVariables\": {\n      \"type\": \"object\",\n      \"description\": \"Expanded\
  \ Call Context (ECC) variables\"\n    },\n    \"transferDestination\": {\n      \"type\": \"string\",\n      \"description\": \"Transfer destination number if the call was transferred\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Error code if the call ended in error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-call-detail-record-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallDetailRecord
---
