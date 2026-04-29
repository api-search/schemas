---
description: WatermarkKey schema from Amazon Elastic Transcoder
layout: schema
name: WatermarkKey
properties_list: []
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-watermark-key-schema.json
slug: amazon-elastic-transcoder-watermark-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-watermark-key-schema.json\",\n  \"title\": \"WatermarkKey\",\n  \"description\": \"WatermarkKey schema from Amazon Elastic Transcoder\",\n  \"type\": \"string\",\n  \"pattern\": \"(^.{1,1020}.jpg$)|(^.{1,1019}.jpeg$)|(^.{1,1020}.png$)\",\n  \"minLength\": 1,\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-watermark-key-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: WatermarkKey
---
