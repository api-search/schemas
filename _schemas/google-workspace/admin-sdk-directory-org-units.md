---
description: A list of organizational unit resources.
layout: schema
name: OrgUnits
properties_list:
- description: The type of the API resource.
  name: kind
  type: string
- description: ETag of the resource.
  name: etag
  type: string
- description: A list of organizational unit objects.
  name: organizationUnits
  type: array
provider_name: Google Workspace
provider_slug: google-workspace
schema_file: json-schema/admin-sdk-directory-org-units-schema.json
slug: admin-sdk-directory-org-units
source_filename: admin-sdk-directory-org-units-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrgUnits\",\n  \"type\": \"object\",\n  \"description\": \"A list of organizational unit resources.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the API resource.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag of the resource.\"\n    },\n    \"organizationUnits\": {\n      \"type\": \"array\",\n      \"description\": \"A list of organizational unit objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/json-schema/admin-sdk-directory-org-units-schema.json
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
title: OrgUnits
---
