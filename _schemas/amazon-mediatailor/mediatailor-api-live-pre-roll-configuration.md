---
description: The configuration for pre-roll ad insertion.
layout: schema
name: LivePreRollConfiguration
properties_list:
- description: ''
  name: AdDecisionServerUrl
  type: object
- description: ''
  name: MaxDurationSeconds
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-live-pre-roll-configuration-schema.json
slug: mediatailor-api-live-pre-roll-configuration
source_filename: mediatailor-api-live-pre-roll-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-live-pre-roll-configuration-schema.json\",\n  \"title\": \"LivePreRollConfiguration\",\n  \"description\": \"The configuration for pre-roll ad insertion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdDecisionServerUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL for the ad decision server (ADS) for pre-roll ads. This includes the specification of static parameters and placeholders for dynamic parameters. AWS Elemental MediaTailor substitutes player-specific and session-specific parameters as needed when calling the ADS. Alternately, for testing, you can provide a static VAST URL. The maximum length is 25,000 characters.\"\n        }\n      ]\n    },\n    \"MaxDurationSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum allowed duration for the pre-roll ad avail. AWS Elemental MediaTailor won't play pre-roll ads to exceed this duration, regardless of the total duration of ads that the ADS returns.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-live-pre-roll-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: LivePreRollConfiguration
---
