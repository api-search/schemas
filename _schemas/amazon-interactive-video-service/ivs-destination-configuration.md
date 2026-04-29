---
description: A complex type that describes a location where recorded videos will be stored. Each member represents a type of destination configuration. For recording, you define one and only one type of destination configuration.
layout: schema
name: DestinationConfiguration
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-destination-configuration-schema.json
slug: ivs-destination-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-destination-configuration-schema.json\",\n  \"title\": \"DestinationConfiguration\",\n  \"description\": \"A complex type that describes a location where recorded videos will be stored. Each member represents a type of destination configuration. For recording, you define one and only one type of destination configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3DestinationConfiguration\"\n        },\n        {\n          \"description\": \"An S3 destination configuration where recorded videos will be stored.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-destination-configuration-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: DestinationConfiguration
---
