---
description: ''
layout: schema
name: CallFlowElement
properties_list:
- description: Name of the call flow element
  name: elementName
  type: string
- description: Type of element. Voice elements interact with the caller, action elements perform backend operations, decision elements control flow logic, and subdialog elements invoke sub-applications.
  name: elementType
  type: string
- description: ''
  name: description
  type: string
- description: Java class implementing the element
  name: className
  type: string
- description: Element-specific configuration
  name: configParameters
  type: object
- description: Element exit paths and their targets
  name: exits
  type: array
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-call-flow-element-schema.json
slug: cisco-voice-portal-vxml-services-call-flow-element
source_filename: cisco-voice-portal-vxml-services-call-flow-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallFlowElement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elementName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the call flow element\"\n    },\n    \"elementType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of element. Voice elements interact with the caller, action elements perform backend operations, decision elements control flow logic, and subdialog elements invoke sub-applications.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"className\": {\n      \"type\": \"string\",\n      \"description\": \"Java class implementing the element\"\n    },\n    \"configParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Element-specific configuration\"\n    },\n    \"exits\": {\n      \"type\": \"array\",\n      \"description\": \"Element exit paths and their targets\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-call-flow-element-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallFlowElement
---
