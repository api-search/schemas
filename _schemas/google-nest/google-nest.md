---
description: JSON Schema for the Google Nest SDM API device, structure, and command objects.
layout: schema
name: Google Nest Smart Device Management API Schema
properties_list: []
provider_name: Google Nest Smart Device Management
provider_slug: google-nest
schema_file: json-schema/google-nest.json
slug: google-nest
source_filename: google-nest.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-nest/refs/heads/main/json-schema/google-nest.json\",\n  \"title\": \"Google Nest Smart Device Management API Schema\",\n  \"description\": \"JSON Schema for the Google Nest SDM API device, structure, and command objects.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"Device\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the device.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Device type identifier.\"\n        },\n        \"traits\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Map of trait names to their current values.\"\n        },\n        \"parentRelations\": {\n          \"type\": \"array\",\n          \"\
  items\": {\n            \"$ref\": \"#/$defs/ParentRelation\"\n          }\n        }\n      }\n    },\n    \"ParentRelation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"parent\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the parent.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the parent.\"\n        }\n      }\n    },\n    \"Structure\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the structure.\"\n        },\n        \"traits\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Structure traits and values.\"\n        }\n      }\n    },\n    \"Room\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Resource name of the room.\"\n        },\n        \"traits\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Room traits and values.\"\n        }\n      }\n    },\n    \"ExecuteCommandRequest\": {\n      \"type\": \"object\",\n      \"required\": [\"command\"],\n      \"properties\": {\n        \"command\": {\n          \"type\": \"string\",\n          \"description\": \"The command to execute.\"\n        },\n        \"params\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Command parameters.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-nest/refs/heads/main/json-schema/google-nest.json
tags:
- Camera
- Device Management
- Doorbell
- Google Nest
- IoT
- Smart Home
- Thermostat
title: Google Nest Smart Device Management API Schema
---
