---
description: Schema for a CVP Dialed Number Pattern (DNP). Dialed number patterns define how incoming calls are routed to specific VXML applications or call treatments based on the dialed number (DNIS). DNPs are a core configuration element in CVP that maps incoming numbers to call handling logic and integrates with ICM/UCCE routing.
layout: schema
name: Cisco Voice Portal Dialed Number Pattern
properties_list:
- description: Unique identifier for the pattern
  name: patternId
  type: string
- description: 'The dialed number pattern. Supports wildcards (* for any digits). Examples: 18005551234, 1800555*, *'
  name: pattern
  type: string
- description: Description of what this pattern routes to
  name: description
  type: string
- description: Call type determining how the call interacts with ICM/UCCE. Pre-route calls are sent to ICM before any treatment. Translation-route calls receive self-service treatment then route to ICM. Post-route c
  name: callType
  type: string
- description: VXML application associated with this pattern
  name: applicationName
  type: string
- description: Whether this pattern is active
  name: enabled
  type: boolean
- description: Pattern matching priority (lower number = higher priority)
  name: priority
  type: integer
- description: SIP server group for outbound routing
  name: sipServerGroup
  type: string
- description: Application to play while waiting for ICM route response
  name: ringtoneApplication
  type: string
- description: Application to play on error conditions
  name: errorApplication
  type: string
- description: Application to use in ICM survival mode (when ICM is unreachable)
  name: survivalApplication
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-dialed-number-pattern.json
slug: cisco-voice-portal-dialed-number-pattern
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-voice-portal/json-schema/cisco-voice-portal-dialed-number-pattern.json\",\n  \"title\": \"Cisco Voice Portal Dialed Number Pattern\",\n  \"description\": \"Schema for a CVP Dialed Number Pattern (DNP). Dialed number patterns define how incoming calls are routed to specific VXML applications or call treatments based on the dialed number (DNIS). DNPs are a core configuration element in CVP that maps incoming numbers to call handling logic and integrates with ICM/UCCE routing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patternId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the pattern\"\n    },\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"The dialed number pattern. Supports wildcards (* for any digits). Examples: 18005551234, 1800555*, *\"\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Description of what this pattern routes to\"\n    },\n    \"callType\": {\n      \"type\": \"string\",\n      \"enum\": [\"preroute\", \"translation_route\", \"post_route\"],\n      \"description\": \"Call type determining how the call interacts with ICM/UCCE. Pre-route calls are sent to ICM before any treatment. Translation-route calls receive self-service treatment then route to ICM. Post-route calls are fully handled by CVP without ICM.\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"VXML application associated with this pattern\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether this pattern is active\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Pattern matching priority (lower number = higher priority)\"\n    },\n    \"sipServerGroup\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"SIP server group for outbound routing\"\n    },\n    \"ringtoneApplication\": {\n      \"type\": \"string\",\n      \"description\": \"Application to play while waiting for ICM route response\"\n    },\n    \"errorApplication\": {\n      \"type\": \"string\",\n      \"description\": \"Application to play on error conditions\"\n    },\n    \"survivalApplication\": {\n      \"type\": \"string\",\n      \"description\": \"Application to use in ICM survival mode (when ICM is unreachable)\"\n    }\n  },\n  \"required\": [\"pattern\", \"callType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-dialed-number-pattern.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: Cisco Voice Portal Dialed Number Pattern
---
