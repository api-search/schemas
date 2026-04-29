---
description: The configuration for avail suppression, also known as ad suppression. For more information about ad suppression, see <a href="https://docs.aws.amazon.com/mediatailor/latest/ug/ad-behavior.html">Ad Suppression</a>.
layout: schema
name: AvailSuppression
properties_list:
- description: ''
  name: Mode
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-avail-suppression-schema.json
slug: mediatailor-api-avail-suppression
source_filename: mediatailor-api-avail-suppression-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-avail-suppression-schema.json\",\n  \"title\": \"AvailSuppression\",\n  \"description\": \"The configuration for avail suppression, also known as ad suppression. For more information about ad suppression, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/ad-behavior.html\\\">Ad Suppression</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mode\"\n        },\n        {\n          \"description\": \"Sets the ad suppression mode. By default, ad suppression is off and all ad breaks are filled with ads or slate. When Mode is set to <code>BEHIND_LIVE_EDGE</code>, ad suppression is active and MediaTailor won't fill ad breaks on or behind the ad suppression Value time in the manifest\
  \ lookback window.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A live edge offset time in HH:MM:SS. MediaTailor won't fill ad breaks on or behind this time in the manifest lookback window. If Value is set to 00:00:00, it is in sync with the live edge, and MediaTailor won't fill any ad breaks on or behind the live edge. If you set a Value time, MediaTailor won't fill any ad breaks on or behind this time in the manifest lookback window. For example, if you set 00:45:00, then MediaTailor will fill ad breaks that occur within 45 minutes behind the live edge, but won't fill ad breaks on or behind 45 minutes behind the live edge.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-avail-suppression-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvailSuppression
---
