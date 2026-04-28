---
description: Schema for a search rule configuration on Cisco Expressway. Search rules define how the Expressway routes incoming search requests to the appropriate target zones or policy services based on alias pattern matching, source zone, and protocol filtering.
layout: schema
name: Cisco Expressway Search Rule
properties_list:
- description: Unique name for the search rule
  name: Name
  type: string
- description: Priority of the search rule. Lower numbers are evaluated first. Rules with the same priority are evaluated in parallel.
  name: Priority
  type: integer
- description: Type of pattern matching to apply to the destination alias
  name: AliasPatternType
  type: string
- description: 'The pattern to match against the destination alias. Format depends on AliasPatternType: literal string for Prefix/Suffix/Exact, regular expression for Regex.'
  name: AliasPatternString
  type: string
- description: Name of the zone to which matching search requests are forwarded
  name: TargetZone
  type: string
- description: Name of the source zone from which requests must originate for this rule to apply. When empty or not set, requests from any zone match.
  name: SourceZone
  type: string
- description: Whether the search rule is enabled and actively used for routing decisions
  name: Mode
  type: string
- description: Protocol filter. Only requests using the specified protocol will match this rule.
  name: Protocol
  type: string
- description: Action to take when a matching alias is found in the target zone. Stop prevents further search rules from being evaluated. Continue allows lower-priority rules to also be evaluated.
  name: OnSuccessfulMatch
  type: string
- description: Optional description of the search rule's purpose and behavior
  name: Description
  type: string
- description: Administrative state of the search rule
  name: State
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-search-rule-schema.json
slug: cisco-expressway-search-rule
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Search Rule
---
