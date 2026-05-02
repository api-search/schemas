---
description: Represents the permissions configuration for a Looker Studio asset, mapping roles to arrays of member identifiers. Used for managing sharing and access control on reports and data sources.
layout: schema
name: Looker Studio Permissions
properties_list:
- description: A mapping of roles to arrays of member identifiers. Each key is a role (VIEWER, EDITOR, OWNER, LINK_VIEWER, LINK_EDITOR) and each value is an array of member strings using prefixed format.
  name: permissions
  type: object
- description: An opaque string used for optimistic concurrency control. Include this value in update requests to prevent conflicting modifications.
  name: etag
  type: string
provider_name: Looker Studio
provider_slug: looker-studio
schema_file: json-schema/looker-studio-permissions-schema.json
slug: looker-studio-permissions
source_filename: looker-studio-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/looker-studio/json-schema/looker-studio-permissions-schema.json\",\n  \"title\": \"Looker Studio Permissions\",\n  \"description\": \"Represents the permissions configuration for a Looker Studio asset, mapping roles to arrays of member identifiers. Used for managing sharing and access control on reports and data sources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissions\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping of roles to arrays of member identifiers. Each key is a role (VIEWER, EDITOR, OWNER, LINK_VIEWER, LINK_EDITOR) and each value is an array of member strings using prefixed format.\",\n      \"properties\": {\n        \"VIEWER\": {\n          \"type\": \"array\",\n          \"description\": \"Members with view-only access to the asset.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Member\"\n    \
  \      }\n        },\n        \"EDITOR\": {\n          \"type\": \"array\",\n          \"description\": \"Members with edit access to the asset.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Member\"\n          }\n        },\n        \"OWNER\": {\n          \"type\": \"array\",\n          \"description\": \"Members with full ownership and control over the asset.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Member\"\n          }\n        },\n        \"LINK_VIEWER\": {\n          \"type\": \"array\",\n          \"description\": \"Members who can view the asset via a shared link.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Member\"\n          }\n        },\n        \"LINK_EDITOR\": {\n          \"type\": \"array\",\n          \"description\": \"Members who can edit the asset via a shared link.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Member\"\n          }\n        }\n      },\n      \"additionalProperties\": false\n    },\n \
  \   \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"An opaque string used for optimistic concurrency control. Include this value in update requests to prevent conflicting modifications.\"\n    }\n  },\n  \"required\": [\n    \"permissions\"\n  ],\n  \"$defs\": {\n    \"Member\": {\n      \"type\": \"string\",\n      \"description\": \"A member identifier using a prefixed format. Supported prefixes: user: (Google account), group: (Google Group), domain: (organizational domain), serviceAccount: (service account), or the literal 'allUsers' for anyone with a link.\",\n      \"examples\": [\n        \"user:jane@example.com\",\n        \"group:team@googlegroups.com\",\n        \"domain:example.com\",\n        \"serviceAccount:bot@project.iam.gserviceaccount.com\",\n        \"allUsers\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/json-schema/looker-studio-permissions-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
title: Looker Studio Permissions
---
