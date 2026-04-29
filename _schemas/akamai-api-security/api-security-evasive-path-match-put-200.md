---
description: The PUT Response JSON for Evasive Path Match.
layout: schema
name: evasive-path-match-put-200
properties_list:
- description: When enabled, evaluates requests with the following list of characters removed ` & ! $ ' ( ) + , [ ] * @ ^ \ "` and `.` only when it appears as a trailing character at the end of the URL. This feature
  name: enablePathMatch
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-evasive-path-match-put-200-schema.json
slug: api-security-evasive-path-match-put-200
source_filename: api-security-evasive-path-match-put-200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-evasive-path-match-put-200-schema.json\",\n  \"title\": \"evasive-path-match-put-200\",\n  \"description\": \"The PUT Response JSON for Evasive Path Match.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enablePathMatch\": {\n      \"description\": \"When enabled, evaluates requests with the following list of characters removed ` & ! $ ' ( ) + , [ ] * @ ^ \\\\ \\\"` and `.` only when it appears as a trailing character at the end of the URL.  This feature does not match on characters that are an integral part of URL requests, like: ``` :  /  #  &  ;  = ``` and `.` when it appears inside the URL string.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"enablePathMatch\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-evasive-path-match-put-200-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: evasive-path-match-put-200
---
