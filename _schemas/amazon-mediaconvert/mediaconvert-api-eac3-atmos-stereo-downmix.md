---
description: 'Choose how the service does stereo downmixing. Default value: Not indicated (ATMOS_STORAGE_DDP_DMIXMOD_NOT_INDICATED) Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the setting Downmix control (DownmixControl). Otherwise, MediaConvert ignores Stereo downmix (StereoDownmix).'
layout: schema
name: Eac3AtmosStereoDownmix
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-atmos-stereo-downmix-schema.json
slug: mediaconvert-api-eac3-atmos-stereo-downmix
source_filename: mediaconvert-api-eac3-atmos-stereo-downmix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-stereo-downmix-schema.json\",\n  \"title\": \"Eac3AtmosStereoDownmix\",\n  \"description\": \"Choose how the service does stereo downmixing. Default value: Not indicated (ATMOS_STORAGE_DDP_DMIXMOD_NOT_INDICATED) Related setting: To have MediaConvert use this value, keep the default value, Custom (SPECIFIED) for the setting Downmix control (DownmixControl). Otherwise, MediaConvert ignores Stereo downmix (StereoDownmix).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NOT_INDICATED\",\n    \"STEREO\",\n    \"SURROUND\",\n    \"DPL2\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-stereo-downmix-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3AtmosStereoDownmix
---
