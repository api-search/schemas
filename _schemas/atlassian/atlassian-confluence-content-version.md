---
description: ''
layout: schema
name: Version
properties_list:
- description: ''
  name: when
  type: string
- description: ''
  name: friendlyWhen
  type: string
- description: ''
  name: message
  type: string
- description: Set this to the current version number incremented by one
  name: number
  type: integer
- description: If `minorEdit` is set to 'true', no notification email or activity stream will be generated for the change.
  name: minorEdit
  type: boolean
- description: ''
  name: _expandable
  type: object
- description: True if content type is modifed in this version (e.g. page to blog)
  name: contentTypeModified
  type: boolean
- description: The revision id provided by confluence to be used as a revision in Synchrony
  name: confRev
  type: string
- description: The revision id provided by Synchrony
  name: syncRev
  type: string
- description: Source of the synchrony revision
  name: syncRevSource
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-version-schema.json
slug: atlassian-confluence-content-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Version\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"when\": {\n      \"type\": \"string\"\n    },\n    \"friendlyWhen\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"Set this to the current version number incremented by one\"\n    },\n    \"minorEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"If `minorEdit` is set to 'true', no notification email or activity\\nstream will be generated for the change.\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    },\n    \"contentTypeModified\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if content type is modifed in this version (e.g. page to blog)\"\n    },\n    \"confRev\": {\n      \"type\": \"string\",\n      \"description\": \"The revision id provided by confluence\
  \ to be used as a revision in Synchrony\"\n    },\n    \"syncRev\": {\n      \"type\": \"string\",\n      \"description\": \"The revision id provided by Synchrony\"\n    },\n    \"syncRevSource\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the synchrony revision\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-version-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Version
---
