---
description: Ttml Destination Settings
layout: schema
name: TtmlDestinationSettings
properties_list:
- description: ''
  name: StyleControl
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-ttml-destination-settings-schema.json
slug: medialive-api-ttml-destination-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ttml-destination-settings-schema.json\",\n  \"title\": \"TtmlDestinationSettings\",\n  \"description\": \"Ttml Destination Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StyleControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TtmlDestinationStyleControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"styleControl\"\n          },\n          \"description\": \"This field is not currently supported and will not affect the output styling. Leave the default value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ttml-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TtmlDestinationSettings
---
