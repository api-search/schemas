---
description: UpdateScriptOutput schema from Amazon GameLift API
layout: schema
name: UpdateScriptOutput
properties_list:
- description: ''
  name: Script
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-script-output-schema.json
slug: gamelift-update-script-output
source_filename: gamelift-update-script-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-script-output-schema.json\",\n  \"title\": \"UpdateScriptOutput\",\n  \"description\": \"UpdateScriptOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Script\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Script\"\n        },\n        {\n          \"description\": \"The newly created script record with a unique script ID. The new script's storage location reflects an Amazon S3 location: (1) If the script was uploaded from an S3 bucket under your account, the storage location reflects the information that was provided in the <i>CreateScript</i> request; (2) If the script file was uploaded from a local zip file, the storage location reflects an S3 location controls by the Amazon GameLift service.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-script-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateScriptOutput
---
