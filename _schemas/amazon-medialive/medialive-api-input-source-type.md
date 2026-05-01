---
description: There are two types of input sources, static and dynamic. If an input source is dynamic you can change the source url of the input dynamically using an input switch action. Currently, two input types support a dynamic url at this time, MP4_FILE and TS_FILE. By default all input sources are static.
layout: schema
name: InputSourceType
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-source-type-schema.json
slug: medialive-api-input-source-type
source_filename: medialive-api-input-source-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-source-type-schema.json\",\n  \"title\": \"InputSourceType\",\n  \"description\": \"There are two types of input sources, static and dynamic. If an input source is dynamic you can\\nchange the source url of the input dynamically using an input switch action. Currently, two input types\\nsupport a dynamic url at this time, MP4_FILE and TS_FILE. By default all input sources are static.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"STATIC\",\n    \"DYNAMIC\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-source-type-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputSourceType
---
