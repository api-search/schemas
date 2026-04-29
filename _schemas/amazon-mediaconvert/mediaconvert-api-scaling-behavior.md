---
description: Specify how the service handles outputs that have a different aspect ratio from the input aspect ratio. Choose Stretch to output (STRETCH_TO_OUTPUT) to have the service stretch your video image to fit. Keep the setting Default (DEFAULT) to have the service letterbox your video instead. This setting overrides any value that you specify for the setting Selection placement (position) in this output.
layout: schema
name: ScalingBehavior
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-scaling-behavior-schema.json
slug: mediaconvert-api-scaling-behavior
source_filename: mediaconvert-api-scaling-behavior-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-scaling-behavior-schema.json\",\n  \"title\": \"ScalingBehavior\",\n  \"description\": \"Specify how the service handles outputs that have a different aspect ratio from the input aspect ratio. Choose Stretch to output (STRETCH_TO_OUTPUT) to have the service stretch your video image to fit. Keep the setting Default (DEFAULT) to have the service letterbox your video instead. This setting overrides any value that you specify for the setting Selection placement (position) in this output.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DEFAULT\",\n    \"STRETCH_TO_OUTPUT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-scaling-behavior-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ScalingBehavior
---
