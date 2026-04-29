---
description: The settings for Automatic Input Failover.
layout: schema
name: AutomaticInputFailoverSettings
properties_list:
- description: ''
  name: ErrorClearTimeMsec
  type: object
- description: ''
  name: FailoverConditions
  type: object
- description: ''
  name: InputPreference
  type: object
- description: ''
  name: SecondaryInputId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-automatic-input-failover-settings-schema.json
slug: medialive-api-automatic-input-failover-settings
source_filename: medialive-api-automatic-input-failover-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-automatic-input-failover-settings-schema.json\",\n  \"title\": \"AutomaticInputFailoverSettings\",\n  \"description\": \"The settings for Automatic Input Failover.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorClearTimeMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorClearTimeMsec\"\n          },\n          \"description\": \"This clear time defines the requirement a recovered input must meet to be considered healthy. The input must have no failover conditions for this length of time. Enter a time in milliseconds. This value is particularly important if the input_preference for the failover pair is set to PRIMARY_INPUT_PREFERRED, because after this\
  \ time, MediaLive will switch back to the primary input.\"\n        }\n      ]\n    },\n    \"FailoverConditions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfFailoverCondition\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"failoverConditions\"\n          },\n          \"description\": \"A list of failover conditions. If any of these conditions occur, MediaLive will perform a failover to the other input.\"\n        }\n      ]\n    },\n    \"InputPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPreference\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputPreference\"\n          },\n          \"description\": \"Input preference when deciding which input to make active when a previously failed input has recovered.\"\n        }\n      ]\n    },\n    \"SecondaryInputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"secondaryInputId\"\n          },\n          \"description\": \"The input ID of the secondary input in the automatic input failover pair.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SecondaryInputId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-automatic-input-failover-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AutomaticInputFailoverSettings
---
