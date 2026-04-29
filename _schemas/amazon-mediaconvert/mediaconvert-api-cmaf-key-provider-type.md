---
description: Specify whether your DRM encryption key is static or from a key provider that follows the SPEKE standard. For more information about SPEKE, see https://docs.aws.amazon.com/speke/latest/documentation/what-is-speke.html.
layout: schema
name: CmafKeyProviderType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-key-provider-type-schema.json
slug: mediaconvert-api-cmaf-key-provider-type
source_filename: mediaconvert-api-cmaf-key-provider-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-key-provider-type-schema.json\",\n  \"title\": \"CmafKeyProviderType\",\n  \"description\": \"Specify whether your DRM encryption key is static or from a key provider that follows the SPEKE standard. For more information about SPEKE, see https://docs.aws.amazon.com/speke/latest/documentation/what-is-speke.html.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SPEKE\",\n    \"STATIC_KEY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-key-provider-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafKeyProviderType
---
