---
description: A Google Workspace organizational unit. JSON representation of an org unit resource from the Admin SDK Directory API. The hierarchy is limited to 35 levels of depth.
layout: schema
name: OrgUnit
properties_list:
- description: The type of the API resource.
  name: kind
  type: string
- description: ETag of the resource.
  name: etag
  type: string
- description: The organizational unit path name. For example, an organizational unit with parent path /corp and name sales is derived as /corp/sales.
  name: name
  type: string
- description: Description of the organizational unit.
  name: description
  type: string
- description: The full path to the organizational unit. The orgUnitPath is a derived property. When listed, it is derived from parentOrgUnitPath and the organizational unit name.
  name: orgUnitPath
  type: string
- description: The unique ID of the organizational unit.
  name: orgUnitId
  type: string
- description: The organizational unit path of the parent organizational unit. Required unless parentOrgUnitId is set.
  name: parentOrgUnitPath
  type: string
- description: The unique ID of the parent organizational unit. Required unless parentOrgUnitPath is set.
  name: parentOrgUnitId
  type: string
- description: Deprecated. Setting this field has no effect.
  name: blockInheritance
  type: boolean
provider_name: Google Workspace
provider_slug: google-workspace
schema_file: json-schema/admin-sdk-directory-org-unit-schema.json
slug: admin-sdk-directory-org-unit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrgUnit\",\n  \"type\": \"object\",\n  \"description\": \"A Google Workspace organizational unit. JSON representation of an org unit resource from the Admin SDK Directory API. The hierarchy is limited to 35 levels of depth.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the API resource.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag of the resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The organizational unit path name. For example, an organizational unit with parent path /corp and name sales is derived as /corp/sales.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the organizational unit.\"\n    },\n    \"orgUnitPath\": {\n      \"type\": \"string\",\n      \"description\": \"The full path\
  \ to the organizational unit. The orgUnitPath is a derived property. When listed, it is derived from parentOrgUnitPath and the organizational unit name.\"\n    },\n    \"orgUnitId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the organizational unit.\"\n    },\n    \"parentOrgUnitPath\": {\n      \"type\": \"string\",\n      \"description\": \"The organizational unit path of the parent organizational unit. Required unless parentOrgUnitId is set.\"\n    },\n    \"parentOrgUnitId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the parent organizational unit. Required unless parentOrgUnitPath is set.\"\n    },\n    \"blockInheritance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deprecated. Setting this field has no effect.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/json-schema/admin-sdk-directory-org-unit-schema.json
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
title: OrgUnit
---
