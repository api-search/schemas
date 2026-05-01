---
description: The current state of the multiplex.
layout: schema
name: MultiplexState
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-state-schema.json
slug: medialive-api-multiplex-state
source_filename: medialive-api-multiplex-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-state-schema.json\",\n  \"title\": \"MultiplexState\",\n  \"description\": \"The current state of the multiplex.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREATING\",\n    \"CREATE_FAILED\",\n    \"IDLE\",\n    \"STARTING\",\n    \"RUNNING\",\n    \"RECOVERING\",\n    \"STOPPING\",\n    \"DELETING\",\n    \"DELETED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-state-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MultiplexState
---
