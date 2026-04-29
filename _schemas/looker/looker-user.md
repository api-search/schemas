---
description: A Looker user account. Users have credentials, roles, and can own content such as Looks, dashboards, and queries.
layout: schema
name: User
properties_list:
- description: Unique numeric identifier
  name: id
  type: integer
- description: First name
  name: first_name
  type: string
- description: Last name
  name: last_name
  type: string
- description: Full display name
  name: display_name
  type: string
- description: Email address
  name: email
  type: string
- description: URL of the user's avatar image
  name: avatar_url
  type: string
- description: Whether the user account is disabled
  name: is_disabled
  type: boolean
- description: User's locale setting
  name: locale
  type: string
- description: ID of the user's personal space (folder)
  name: home_space_id
  type: string
- description: ID of the user's personal folder
  name: home_folder_id
  type: string
- description: ID of the user's personal space
  name: personal_space_id
  type: integer
- description: ID of the user's personal folder
  name: personal_folder_id
  type: integer
- description: Whether the user is a Looker employee
  name: presumed_looker_employee
  type: boolean
- description: Whether the user is a verified Looker employee
  name: verified_looker_employee
  type: boolean
- description: Whether user roles are managed externally (e.g. via SAML)
  name: roles_externally_managed
  type: boolean
- description: Whether roles can be assigned directly to this user
  name: allow_direct_roles
  type: boolean
- description: Whether the user can be added to groups
  name: allow_normal_group_membership
  type: boolean
- description: Whether the user inherits roles from groups
  name: allow_roles_from_normal_groups
  type: boolean
- description: Embed group space ID
  name: embed_group_space_id
  type: integer
- description: API3 credentials for this user
  name: credentials_api3
  type: array
- description: Active sessions for this user
  name: sessions
  type: array
- description: IDs of roles assigned to this user
  name: role_ids
  type: array
- description: IDs of groups this user belongs to
  name: group_ids
  type: array
- description: Relative URL for this user
  name: url
  type: string
- description: Timestamp when the user was created
  name: created_at
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-user-schema.json
slug: looker-user
source_filename: looker-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A Looker user account. Users have credentials, roles, and can own content such as Looks, dashboards, and queries.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the user's avatar image\"\n    },\n    \"is_disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the user account is disabled\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"User's locale setting\"\n    },\n    \"home_space_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user's personal space (folder)\"\n    },\n    \"home_folder_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user's personal folder\"\n    },\n    \"personal_space_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user's personal space\"\n    },\n    \"personal_folder_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user's personal folder\"\n    },\n    \"presumed_looker_employee\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a Looker employee\"\n    },\n    \"verified_looker_employee\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a verified Looker employee\"\n    },\n    \"roles_externally_managed\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Whether user roles are managed externally (e.g. via SAML)\"\n    },\n    \"allow_direct_roles\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether roles can be assigned directly to this user\"\n    },\n    \"allow_normal_group_membership\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can be added to groups\"\n    },\n    \"allow_roles_from_normal_groups\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user inherits roles from groups\"\n    },\n    \"embed_group_space_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Embed group space ID\"\n    },\n    \"credentials_api3\": {\n      \"type\": \"array\",\n      \"description\": \"API3 credentials for this user\"\n    },\n    \"sessions\": {\n      \"type\": \"array\",\n      \"description\": \"Active sessions for this user\"\n    },\n    \"role_ids\": {\n      \"type\": \"array\",\n      \"description\": \"\
  IDs of roles assigned to this user\"\n    },\n    \"group_ids\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of groups this user belongs to\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL for this user\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the user was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-user-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: User
---
