---
description: Represents the Profile and Tier, per the HEVC (H.265) specification. Selections are grouped as [Profile] / [Tier], so "Main/High" represents Main Profile with High Tier. 4:2:2 profiles are only available with the HEVC 4:2:2 License.
layout: schema
name: H265CodecProfile
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h265-codec-profile-schema.json
slug: mediaconvert-api-h265-codec-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-codec-profile-schema.json\",\n  \"title\": \"H265CodecProfile\",\n  \"description\": \"Represents the Profile and Tier, per the HEVC (H.265) specification. Selections are grouped as [Profile] / [Tier], so \\\"Main/High\\\" represents Main Profile with High Tier. 4:2:2 profiles are only available with the HEVC 4:2:2 License.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"MAIN_MAIN\",\n    \"MAIN_HIGH\",\n    \"MAIN10_MAIN\",\n    \"MAIN10_HIGH\",\n    \"MAIN_422_8BIT_MAIN\",\n    \"MAIN_422_8BIT_HIGH\",\n    \"MAIN_422_10BIT_MAIN\",\n    \"MAIN_422_10BIT_HIGH\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-codec-profile-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H265CodecProfile
---
