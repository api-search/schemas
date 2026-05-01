---
description: Settings for your Nielsen configuration. If you don't do Nielsen measurement and analytics, ignore these settings. When you enable Nielsen configuration (nielsenConfiguration), MediaConvert enables PCM to ID3 tagging for all outputs in the job. To enable Nielsen configuration programmatically, include an instance of nielsenConfiguration in your JSON job specification. Even if you don't include any children of nielsenConfiguration, you still enable the setting.
layout: schema
name: NielsenConfiguration
properties_list:
- description: ''
  name: BreakoutCode
  type: object
- description: ''
  name: DistributorId
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-nielsen-configuration-schema.json
slug: mediaconvert-api-nielsen-configuration
source_filename: mediaconvert-api-nielsen-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-configuration-schema.json\",\n  \"title\": \"NielsenConfiguration\",\n  \"description\": \"Settings for your Nielsen configuration. If you don't do Nielsen measurement and analytics, ignore these settings. When you enable Nielsen configuration (nielsenConfiguration), MediaConvert enables PCM to ID3 tagging for all outputs in the job. To enable Nielsen configuration programmatically, include an instance of nielsenConfiguration in your JSON job specification. Even if you don't include any children of nielsenConfiguration, you still enable the setting.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BreakoutCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max0\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"breakoutCode\"\n          },\n          \"description\": \"Nielsen has discontinued the use of breakout code functionality. If you must include this property, set the value to zero.\"\n        }\n      ]\n    },\n    \"DistributorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"distributorId\"\n          },\n          \"description\": \"Use Distributor ID (DistributorID) to specify the distributor ID that is assigned to your organization by Neilsen.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-configuration-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NielsenConfiguration
---
