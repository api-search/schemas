---
description: The configuration for manifest processing rules. Manifest processing rules enable customization of the personalized manifests created by MediaTailor.
layout: schema
name: ManifestProcessingRules
properties_list:
- description: ''
  name: AdMarkerPassthrough
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-manifest-processing-rules-schema.json
slug: mediatailor-api-manifest-processing-rules
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-manifest-processing-rules-schema.json\",\n  \"title\": \"ManifestProcessingRules\",\n  \"description\": \"The configuration for manifest processing rules. Manifest processing rules enable customization of the personalized manifests created by MediaTailor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdMarkerPassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdMarkerPassthrough\"\n        },\n        {\n          \"description\": \"<p>For HLS, when set to <code>true</code>, MediaTailor passes through <code>EXT-X-CUE-IN</code>, <code>EXT-X-CUE-OUT</code>, and <code>EXT-X-SPLICEPOINT-SCTE35</code> ad markers from the origin manifest to the MediaTailor personalized manifest.</p> <p>No logic is applied to these ad markers. For example, if\
  \ <code>EXT-X-CUE-OUT</code> has a value of <code>60</code>, but no ads are filled for that ad break, MediaTailor will not set the value to <code>0</code>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-manifest-processing-rules-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ManifestProcessingRules
---
