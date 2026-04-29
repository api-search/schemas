---
description: A list of SCTE-35 message types that are treated as ad markers in the output. If empty, no ad markers are output. Specify multiple items to create ad markers for all of the included message types.
layout: schema
name: AdTriggers
properties_list: []
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-ad-triggers-schema.json
slug: mediapackage-api-ad-triggers
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-ad-triggers-schema.json\",\n  \"title\": \"AdTriggers\",\n  \"description\": \"A list of SCTE-35 message types that are treated as ad markers in the output.  If empty, no\\nad markers are output.  Specify multiple items to create ad markers for all of the included\\nmessage types.\\n\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/__AdTriggersElement\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-ad-triggers-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AdTriggers
---
