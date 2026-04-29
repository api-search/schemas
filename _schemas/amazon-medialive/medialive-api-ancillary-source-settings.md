---
description: Ancillary Source Settings
layout: schema
name: AncillarySourceSettings
properties_list:
- description: ''
  name: SourceAncillaryChannelNumber
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-ancillary-source-settings-schema.json
slug: medialive-api-ancillary-source-settings
source_filename: medialive-api-ancillary-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ancillary-source-settings-schema.json\",\n  \"title\": \"AncillarySourceSettings\",\n  \"description\": \"Ancillary Source Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceAncillaryChannelNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max4\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceAncillaryChannelNumber\"\n          },\n          \"description\": \"Specifies the number (1 to 4) of the captions channel you want to extract from the ancillary captions. If you plan to convert the ancillary captions to another format, complete this field. If you plan to choose Embedded as the captions destination in the output (to pass through all the channels in the ancillary captions), leave this field\
  \ blank because MediaLive ignores the field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ancillary-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AncillarySourceSettings
---
