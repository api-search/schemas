---
description: Access control configuration for a Looker Studio asset. Contains a mapping of roles to their assigned members and an etag for optimistic concurrency control to detect concurrent modifications.
layout: schema
name: Looker Studio Permissions
properties_list:
- description: A map of role names to their member lists. Roles include OWNER, EDITOR, VIEWER, LINK_VIEWER, and LINK_EDITOR.
  name: permissions
  type: object
- description: Etag for optimistic concurrency control. Include this value in PATCH requests to detect and fail on concurrent modifications.
  name: etag
  type: string
provider_name: Google Data Studio
provider_slug: google-data-studio
schema_file: json-schema/google-data-studio-permissions-schema.json
slug: google-data-studio-permissions
source_filename: google-data-studio-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"google-data-studio-permissions-schema.json\",\n  \"title\": \"Looker Studio Permissions\",\n  \"description\": \"Access control configuration for a Looker Studio asset. Contains a mapping of roles to their assigned members and an etag for optimistic concurrency control to detect concurrent modifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissions\": {\n      \"type\": \"object\",\n      \"description\": \"A map of role names to their member lists. Roles include OWNER, EDITOR, VIEWER, LINK_VIEWER, and LINK_EDITOR.\",\n      \"properties\": {\n        \"OWNER\": {\n          \"$ref\": \"#/$defs/RoleMembers\"\n        },\n        \"EDITOR\": {\n          \"$ref\": \"#/$defs/RoleMembers\"\n        },\n        \"VIEWER\": {\n          \"$ref\": \"#/$defs/RoleMembers\"\n        },\n        \"LINK_VIEWER\": {\n          \"$ref\": \"#/$defs/RoleMembers\"\n        },\n        \"\
  LINK_EDITOR\": {\n          \"$ref\": \"#/$defs/RoleMembers\"\n        }\n      },\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/RoleMembers\"\n      }\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Etag for optimistic concurrency control. Include this value in PATCH requests to detect and fail on concurrent modifications.\"\n    }\n  },\n  \"$defs\": {\n    \"RoleMembers\": {\n      \"type\": \"object\",\n      \"description\": \"A list of members assigned to a particular role.\",\n      \"properties\": {\n        \"members\": {\n          \"type\": \"array\",\n          \"description\": \"List of member identifiers with type prefixes.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Member\"\n          }\n        }\n      },\n      \"required\": [\n        \"members\"\n      ]\n    },\n    \"Member\": {\n      \"type\": \"string\",\n      \"description\": \"A member identifier with a type prefix. Supported formats: user:email@example.com\
  \ (Google account), group:group@googlegroups.com (Google Group), domain:example.com (organization domain), serviceAccount:sa@project.iam.gserviceaccount.com (Cloud service account), and allUsers (anyone with the link).\",\n      \"examples\": [\n        \"user:gus@gmail.com\",\n        \"group:api@googlegroups.com\",\n        \"domain:example.com\",\n        \"serviceAccount:sa@project.iam.gserviceaccount.com\",\n        \"allUsers\"\n      ]\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/json-schema/google-data-studio-permissions-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
title: Looker Studio Permissions
---
