---
description: ''
layout: schema
name: RoutingResult
properties_list:
- description: ''
  name: dialedNumber
  type: string
- description: Whether a matching pattern was found
  name: matched
  type: boolean
- description: The dialed number pattern that matched
  name: matchedPattern
  type: string
- description: ''
  name: callType
  type: string
- description: Application that would handle the call
  name: applicationName
  type: string
- description: Resulting route destination
  name: routeDestination
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-routing-result-schema.json
slug: cisco-voice-portal-call-control-routing-result
source_filename: cisco-voice-portal-call-control-routing-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoutingResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dialedNumber\": {\n      \"type\": \"string\"\n    },\n    \"matched\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a matching pattern was found\"\n    },\n    \"matchedPattern\": {\n      \"type\": \"string\",\n      \"description\": \"The dialed number pattern that matched\"\n    },\n    \"callType\": {\n      \"type\": \"string\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Application that would handle the call\"\n    },\n    \"routeDestination\": {\n      \"type\": \"string\",\n      \"description\": \"Resulting route destination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-routing-result-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: RoutingResult
---
