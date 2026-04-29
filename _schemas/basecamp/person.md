---
description: ''
layout: schema
name: Person
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/person-schema.json
slug: person
source_filename: person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/person-schema.json\",\n  \"title\": \"Person\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/PersonRef\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"can_ping\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the authenticated user can direct message this person\"\n        },\n        \"can_manage_projects\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the person can manage projects\"\n        },\n        \"can_manage_people\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the person can manage people\"\n        },\n        \"can_access_timesheet\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the person can access timesheets\"\n        },\n        \"can_access_hill_charts\":\
  \ {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the person can access hill charts\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/person-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Person
---
