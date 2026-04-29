---
description: Groups objects to create an object group.
layout: schema
name: GroupObjectsRequest
properties_list:
- description: A user-supplied object ID for the group to be created.
  name: groupObjectId
  type: string
- description: The object IDs of the objects to group.
  name: childrenObjectIds
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-group-objects-request-schema.json
slug: google-slides-group-objects-request
source_filename: google-slides-group-objects-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupObjectsRequest\",\n  \"type\": \"object\",\n  \"description\": \"Groups objects to create an object group.\",\n  \"properties\": {\n    \"groupObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID for the group to be created.\"\n    },\n    \"childrenObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"The object IDs of the objects to group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-group-objects-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: GroupObjectsRequest
---
