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
