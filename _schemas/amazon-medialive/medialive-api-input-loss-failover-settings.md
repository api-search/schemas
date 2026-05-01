---
description: MediaLive will perform a failover if content is not detected in this input for the specified period.
layout: schema
name: InputLossFailoverSettings
properties_list:
- description: ''
  name: InputLossThresholdMsec
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-loss-failover-settings-schema.json
slug: medialive-api-input-loss-failover-settings
source_filename: medialive-api-input-loss-failover-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-loss-failover-settings-schema.json\",\n  \"title\": \"InputLossFailoverSettings\",\n  \"description\": \"MediaLive will perform a failover if content is not detected in this input for the specified period.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputLossThresholdMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossThresholdMsec\"\n          },\n          \"description\": \"The amount of time (in milliseconds) that no input is detected. After that time, an input failover will occur.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-loss-failover-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputLossFailoverSettings
---
