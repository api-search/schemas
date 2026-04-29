---
description: When you use DRM with CMAF outputs, choose whether the service writes the 128-bit encryption initialization vector in the HLS and DASH manifests.
layout: schema
name: CmafInitializationVectorInManifest
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-initialization-vector-in-manifest-schema.json
slug: mediaconvert-api-cmaf-initialization-vector-in-manifest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-initialization-vector-in-manifest-schema.json\",\n  \"title\": \"CmafInitializationVectorInManifest\",\n  \"description\": \"When you use DRM with CMAF outputs, choose whether the service writes the 128-bit encryption initialization vector in the HLS and DASH manifests.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INCLUDE\",\n    \"EXCLUDE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-initialization-vector-in-manifest-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafInitializationVectorInManifest
---
