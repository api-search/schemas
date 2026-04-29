---
description: Object that describes which renditions should be recorded for a stream.
layout: schema
name: RenditionConfiguration
properties_list:
- description: ''
  name: renditionSelection
  type: object
- description: ''
  name: renditions
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-rendition-configuration-schema.json
slug: ivs-rendition-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-rendition-configuration-schema.json\",\n  \"title\": \"RenditionConfiguration\",\n  \"description\": \"Object that describes which renditions should be recorded for a stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"renditionSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenditionConfigurationRenditionSelection\"\n        },\n        {\n          \"description\": \"Indicates which set of renditions are recorded for a stream. For <code>BASIC</code> channels, the <code>CUSTOM</code> value has no effect. If <code>CUSTOM</code> is specified, a set of renditions must be specified in the <code>renditions</code> field. Default: <code>ALL</code>.\"\n        }\n      ]\n    },\n    \"renditions\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/RenditionConfigurationRenditionList\"\n        },\n        {\n          \"description\": \"Indicates which renditions are recorded for a stream, if <code>renditionSelection</code> is <code>CUSTOM</code>; otherwise, this field is irrelevant. The selected renditions are recorded if they are available during the stream. If a selected rendition is unavailable, the best available rendition is recorded. For details on the resolution dimensions of each rendition, see <a href=\\\"https://docs.aws.amazon.com/ivs/latest/userguide/record-to-s3.html\\\">Auto-Record to Amazon S3</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-rendition-configuration-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: RenditionConfiguration
---
