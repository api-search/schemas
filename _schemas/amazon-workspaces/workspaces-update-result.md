---
description: <p>Describes whether a WorkSpace image needs to be updated with the latest drivers and other components required by Amazon WorkSpaces.</p> <note> <p>Only Windows 10 WorkSpace images can be programmatically updated at this time.</p> </note>
layout: schema
name: UpdateResult
properties_list:
- description: ''
  name: UpdateAvailable
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-update-result-schema.json
slug: workspaces-update-result
source_filename: workspaces-update-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateAvailable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether updated drivers or other components are available for the specified WorkSpace image.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDescription\"\n        },\n        {\n          \"description\": \"A description of whether updates for the WorkSpace image are pending or available.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>Describes whether a WorkSpace image needs to be updated with the latest drivers and other components required by Amazon WorkSpaces.</p> <note> <p>Only Windows 10 WorkSpace images can be programmatically updated at this time.</p> </note>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\":\
  \ \"UpdateResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-result-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UpdateResult
---
