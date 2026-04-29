---
description: Provide the font script, using an ISO 15924 script code, if the LanguageCode is not sufficient for determining the script type. Where LanguageCode or CustomLanguageCode is sufficient, use "AUTOMATIC" or leave unset.
layout: schema
name: FontScript
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-font-script-schema.json
slug: mediaconvert-api-font-script
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-font-script-schema.json\",\n  \"title\": \"FontScript\",\n  \"description\": \"Provide the font script, using an ISO 15924 script code, if the LanguageCode is not sufficient for determining the script type. Where LanguageCode or CustomLanguageCode is sufficient, use \\\"AUTOMATIC\\\" or leave unset.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AUTOMATIC\",\n    \"HANS\",\n    \"HANT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-font-script-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FontScript
---
