---
description: Settings related to teletext captions. Set up teletext captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/teletext-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to TELETEXT.
layout: schema
name: TeletextDestinationSettings
properties_list:
- description: ''
  name: PageNumber
  type: object
- description: ''
  name: PageTypes
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-teletext-destination-settings-schema.json
slug: mediaconvert-api-teletext-destination-settings
source_filename: mediaconvert-api-teletext-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-teletext-destination-settings-schema.json\",\n  \"title\": \"TeletextDestinationSettings\",\n  \"description\": \"Settings related to teletext captions. Set up teletext captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/teletext-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to TELETEXT.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PageNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max3Pattern1809aFAF09aEAE\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pageNumber\"\n          },\n          \"description\": \"Set pageNumber\
  \ to the Teletext page number for the destination captions for this output. This value must be a three-digit hexadecimal string; strings ending in -FF are invalid. If you are passing through the entire set of Teletext data, do not use this field.\"\n        }\n      ]\n    },\n    \"PageTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfTeletextPageType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pageTypes\"\n          },\n          \"description\": \"Specify the page types for this Teletext page. If you don't specify a value here, the service sets the page type to the default value Subtitle (PAGE_TYPE_SUBTITLE). If you pass through the entire set of Teletext data, don't use this field. When you pass through a set of Teletext pages, your output has the same page types as your input.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-teletext-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TeletextDestinationSettings
---
