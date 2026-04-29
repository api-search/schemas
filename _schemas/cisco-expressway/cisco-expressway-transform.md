---
description: Schema for a pre-search transform configuration on Cisco Expressway. Pre-search transforms modify the destination alias in an incoming search request before any searches are performed, enabling alias normalization, number rewriting, and E.164 dialing plan adjustments.
layout: schema
name: Cisco Expressway Pre-Search Transform
properties_list:
- description: Unique name for the transform
  name: Name
  type: string
- description: Priority of the transform. Lower numbers are applied first. Transforms are applied sequentially in priority order.
  name: Priority
  type: integer
- description: Type of pattern matching for the destination alias
  name: PatternType
  type: string
- description: 'The pattern to match against the destination alias. Format depends on PatternType: literal string for Prefix/Suffix/Exact, regular expression for Regex. Regex patterns support capture groups for use i'
  name: PatternString
  type: string
- description: Action to take when the pattern matches the destination alias
  name: PatternBehavior
  type: string
- description: The replacement string applied when the pattern matches. Supports regex capture group references (e.g., \1, \2) when PatternType is Regex.
  name: ReplaceString
  type: string
- description: Administrative state of the transform
  name: State
  type: string
- description: Optional description of the transform's purpose and behavior
  name: Description
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-transform-schema.json
slug: cisco-expressway-transform
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-transform-schema.json\",\n  \"title\": \"Cisco Expressway Pre-Search Transform\",\n  \"description\": \"Schema for a pre-search transform configuration on Cisco Expressway. Pre-search transforms modify the destination alias in an incoming search request before any searches are performed, enabling alias normalization, number rewriting, and E.164 dialing plan adjustments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the transform\",\n      \"minLength\": 1,\n      \"maxLength\": 50,\n      \"examples\": [\"StripPrefix\", \"AddE164Prefix\"]\n    },\n    \"Priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the transform. Lower numbers are applied first. Transforms are applied sequentially in priority order.\"\
  ,\n      \"minimum\": 1,\n      \"maximum\": 65534,\n      \"default\": 1,\n      \"examples\": [1, 10, 50]\n    },\n    \"PatternType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of pattern matching for the destination alias\",\n      \"enum\": [\"Prefix\", \"Suffix\", \"Regex\", \"Exact\"]\n    },\n    \"PatternString\": {\n      \"type\": \"string\",\n      \"description\": \"The pattern to match against the destination alias. Format depends on PatternType: literal string for Prefix/Suffix/Exact, regular expression for Regex. Regex patterns support capture groups for use in ReplaceString.\",\n      \"examples\": [\"9(.*)\", \"^\\\\+1(\\\\d{10})$\", \"0044\"]\n    },\n    \"PatternBehavior\": {\n      \"type\": \"string\",\n      \"description\": \"Action to take when the pattern matches the destination alias\",\n      \"enum\": [\"Replace\", \"Strip\", \"Add Prefix\", \"Add Suffix\"],\n      \"default\": \"Replace\"\n    },\n    \"ReplaceString\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The replacement string applied when the pattern matches. Supports regex capture group references (e.g., \\\\1, \\\\2) when PatternType is Regex.\",\n      \"examples\": [\"\\\\1\", \"+1\\\\1\", \"sip:\\\\1@example.com\"]\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative state of the transform\",\n      \"enum\": [\"Enabled\", \"Disabled\"],\n      \"default\": \"Enabled\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the transform's purpose and behavior\",\n      \"maxLength\": 200\n    }\n  },\n  \"required\": [\"Name\", \"PatternType\", \"PatternString\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-transform-schema.json
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Pre-Search Transform
---
