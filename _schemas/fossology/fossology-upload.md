---
description: A FOSSology upload representing a scanned source artifact.
layout: schema
name: FOSSologyUpload
properties_list:
- description: Unique upload identifier.
  name: id
  type: integer
- description: Parent folder identifier.
  name: folderid
  type: integer
- description: Parent folder name.
  name: foldername
  type: string
- description: Human description of the upload.
  name: description
  type: string
- description: Name assigned to the upload (typically the source filename).
  name: uploadname
  type: string
- description: When the upload was created.
  name: uploaddate
  type: string
- description: User id the upload is assigned to.
  name: assignee
  type: integer
- description: ''
  name: assigneeDate
  type:
  - string
  - 'null'
- description: ''
  name: closingDate
  type:
  - string
  - 'null'
- description: ''
  name: hash
  type: object
- description: ''
  name: filesize
  type: integer
- description: ''
  name: clearingStatus
  type: string
provider_name: FOSSology
provider_slug: fossology
schema_file: json-schema/fossology-upload.json
slug: fossology-upload
source_filename: fossology-upload.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/json-schema/fossology-upload.json\",\n  \"title\": \"FOSSologyUpload\",\n  \"description\": \"A FOSSology upload representing a scanned source artifact.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"foldername\", \"uploadname\"],\n  \"properties\": {\n    \"id\": { \"type\": \"integer\", \"description\": \"Unique upload identifier.\" },\n    \"folderid\": { \"type\": \"integer\", \"description\": \"Parent folder identifier.\" },\n    \"foldername\": { \"type\": \"string\", \"description\": \"Parent folder name.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Human description of the upload.\" },\n    \"uploadname\": { \"type\": \"string\", \"description\": \"Name assigned to the upload (typically the source filename).\" },\n    \"uploaddate\": { \"type\": \"string\", \"format\": \"date-time\"\
  , \"description\": \"When the upload was created.\" },\n    \"assignee\": { \"type\": \"integer\", \"description\": \"User id the upload is assigned to.\" },\n    \"assigneeDate\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n    \"closingDate\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n    \"hash\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sha1\": { \"type\": \"string\" },\n        \"md5\": { \"type\": \"string\" },\n        \"sha256\": { \"type\": \"string\" },\n        \"size\": { \"type\": \"integer\" }\n      }\n    },\n    \"filesize\": { \"type\": \"integer\" },\n    \"clearingStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Open\", \"InProgress\", \"Closed\", \"Rejected\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/json-schema/fossology-upload.json
tags:
- Compliance
- Licensing
- Linux Foundation
- Scanning
- SPDX
- Open Source
title: FOSSologyUpload
---
