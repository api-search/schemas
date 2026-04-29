---
description: Set PSI control (InputPsiControl) for transport stream inputs to specify which data the demux process to scans. * Ignore PSI - Scan all PIDs for audio and video. * Use PSI - Scan only PSI data.
layout: schema
name: InputPsiControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-input-psi-control-schema.json
slug: mediaconvert-api-input-psi-control
source_filename: mediaconvert-api-input-psi-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-psi-control-schema.json\",\n  \"title\": \"InputPsiControl\",\n  \"description\": \"Set PSI control (InputPsiControl) for transport stream inputs to specify which data the demux process to scans. * Ignore PSI - Scan all PIDs for audio and video. * Use PSI - Scan only PSI data.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"IGNORE_PSI\",\n    \"USE_PSI\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-psi-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputPsiControl
---
