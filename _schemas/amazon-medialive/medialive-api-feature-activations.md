---
description: Feature Activations
layout: schema
name: FeatureActivations
properties_list:
- description: ''
  name: InputPrepareScheduleActions
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-feature-activations-schema.json
slug: medialive-api-feature-activations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-feature-activations-schema.json\",\n  \"title\": \"FeatureActivations\",\n  \"description\": \"Feature Activations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputPrepareScheduleActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeatureActivationsInputPrepareScheduleActions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputPrepareScheduleActions\"\n          },\n          \"description\": \"Enables the Input Prepare feature. You can create Input Prepare actions in the schedule only if this feature is enabled.\\nIf you disable the feature on an existing schedule, make sure that you first delete all input prepare actions from the schedule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-feature-activations-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FeatureActivations
---
