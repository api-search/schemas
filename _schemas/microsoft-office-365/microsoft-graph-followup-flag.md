---
description: Allows setting a flag on an item for the user to follow up on later.
layout: schema
name: FollowupFlag
properties_list:
- description: The status of the follow-up flag.
  name: flagStatus
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-followup-flag-schema.json
slug: microsoft-graph-followup-flag
source_filename: microsoft-graph-followup-flag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FollowupFlag\",\n  \"type\": \"object\",\n  \"description\": \"Allows setting a flag on an item for the user to follow up on later.\",\n  \"properties\": {\n    \"flagStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the follow-up flag.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-followup-flag-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: FollowupFlag
---
