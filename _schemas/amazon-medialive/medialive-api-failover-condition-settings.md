---
description: Settings for one failover condition.
layout: schema
name: FailoverConditionSettings
properties_list:
- description: ''
  name: AudioSilenceSettings
  type: object
- description: ''
  name: InputLossSettings
  type: object
- description: ''
  name: VideoBlackSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-failover-condition-settings-schema.json
slug: medialive-api-failover-condition-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-failover-condition-settings-schema.json\",\n  \"title\": \"FailoverConditionSettings\",\n  \"description\": \"Settings for one failover condition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioSilenceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioSilenceFailoverSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSilenceSettings\"\n          },\n          \"description\": \"MediaLive will perform a failover if the specified audio selector is silent for the specified period.\"\n        }\n      ]\n    },\n    \"InputLossSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossFailoverSettings\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"inputLossSettings\"\n          },\n          \"description\": \"MediaLive will perform a failover if content is not detected in this input for the specified period.\"\n        }\n      ]\n    },\n    \"VideoBlackSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoBlackFailoverSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoBlackSettings\"\n          },\n          \"description\": \"MediaLive will perform a failover if content is considered black for the specified period.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-failover-condition-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FailoverConditionSettings
---
