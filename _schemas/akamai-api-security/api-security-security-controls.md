---
description: Describes the operational status of security controls.
layout: schema
name: security-controls
properties_list:
- description: Whether you enabled API constraints.
  name: applyApiConstraints
  type: boolean
- description: Whether you enabled application layer controls.
  name: applyApplicationLayerControls
  type: boolean
- description: Whether you enabled Bot Manager controls.
  name: applyBotmanControls
  type: boolean
- description: Whether you enabled network layer controls.
  name: applyNetworkLayerControls
  type: boolean
- description: Whether you enabled rate controls.
  name: applyRateControls
  type: boolean
- description: Whether you enabled reputation controls.
  name: applyReputationControls
  type: boolean
- description: Whether you enabled slow post controls.
  name: applySlowPostControls
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-security-controls-schema.json
slug: api-security-security-controls
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-security-controls-schema.json\",\n  \"title\": \"security-controls\",\n  \"description\": \"Describes the operational status of security controls.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applyApiConstraints\": {\n      \"description\": \"Whether you enabled API constraints.\",\n      \"type\": \"boolean\"\n    },\n    \"applyApplicationLayerControls\": {\n      \"description\": \"Whether you enabled application layer controls.\",\n      \"type\": \"boolean\"\n    },\n    \"applyBotmanControls\": {\n      \"description\": \"Whether you enabled Bot Manager controls.\",\n      \"type\": \"boolean\"\n    },\n    \"applyNetworkLayerControls\": {\n      \"description\": \"Whether you enabled network layer controls.\",\n      \"type\": \"boolean\"\n    },\n    \"applyRateControls\"\
  : {\n      \"description\": \"Whether you enabled rate controls.\",\n      \"type\": \"boolean\"\n    },\n    \"applyReputationControls\": {\n      \"description\": \"Whether you enabled reputation controls.\",\n      \"type\": \"boolean\"\n    },\n    \"applySlowPostControls\": {\n      \"description\": \"Whether you enabled slow post controls.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"applyApplicationLayerControls\",\n    \"applyNetworkLayerControls\",\n    \"applyRateControls\",\n    \"applyReputationControls\",\n    \"applyBotmanControls\",\n    \"applyApiConstraints\",\n    \"applySlowPostControls\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-security-controls-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: security-controls
---
