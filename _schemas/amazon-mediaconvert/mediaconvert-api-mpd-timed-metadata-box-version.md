---
description: Specify the event message box (eMSG) version for ID3 timed metadata in your output. For more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.3 Syntax. Leave blank to use the default value Version 0. When you specify Version 1, you must also set ID3 metadata (timedMetadata) to Passthrough.
layout: schema
name: MpdTimedMetadataBoxVersion
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mpd-timed-metadata-box-version-schema.json
slug: mediaconvert-api-mpd-timed-metadata-box-version
source_filename: mediaconvert-api-mpd-timed-metadata-box-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-timed-metadata-box-version-schema.json\",\n  \"title\": \"MpdTimedMetadataBoxVersion\",\n  \"description\": \"Specify the event message box (eMSG) version for ID3 timed metadata in your output.\\nFor more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.3 Syntax.\\nLeave blank to use the default value Version 0.\\nWhen you specify Version 1, you must also set ID3 metadata (timedMetadata) to Passthrough.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"VERSION_0\",\n    \"VERSION_1\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-timed-metadata-box-version-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MpdTimedMetadataBoxVersion
---
