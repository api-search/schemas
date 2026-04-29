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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-search-rule-schema.json\",\n  \"title\": \"Cisco Expressway Search Rule\",\n  \"description\": \"Schema for a search rule configuration on Cisco Expressway. Search rules define how the Expressway routes incoming search requests to the appropriate target zones or policy services based on alias pattern matching, source zone, and protocol filtering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the search rule\",\n      \"minLength\": 1,\n      \"maxLength\": 50,\n      \"examples\": [\"Route-to-CUCM\", \"Route-to-DNS\"]\n    },\n    \"Priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the search rule. Lower numbers are evaluated first. Rules with the same priority are evaluated in parallel.\",\n     \
  \ \"minimum\": 1,\n      \"maximum\": 65534,\n      \"default\": 100,\n      \"examples\": [50, 100, 200]\n    },\n    \"AliasPatternType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of pattern matching to apply to the destination alias\",\n      \"enum\": [\"Prefix\", \"Suffix\", \"Regex\", \"Exact\"]\n    },\n    \"AliasPatternString\": {\n      \"type\": \"string\",\n      \"description\": \"The pattern to match against the destination alias. Format depends on AliasPatternType: literal string for Prefix/Suffix/Exact, regular expression for Regex.\",\n      \"examples\": [\".*@example\\\\.com\", \"9011\", \"+1\"]\n    },\n    \"TargetZone\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone to which matching search requests are forwarded\",\n      \"examples\": [\"CUCM-Neighbor\", \"DefaultDNSZone\"]\n    },\n    \"SourceZone\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the source zone from which requests must originate\
  \ for this rule to apply. When empty or not set, requests from any zone match.\",\n      \"examples\": [\"LocalZone\", \"CEtoEXPE-Traversal\"]\n    },\n    \"Mode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the search rule is enabled and actively used for routing decisions\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"On\"\n    },\n    \"Protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol filter. Only requests using the specified protocol will match this rule.\",\n      \"enum\": [\"Any\", \"H.323\", \"SIP\"],\n      \"default\": \"Any\"\n    },\n    \"OnSuccessfulMatch\": {\n      \"type\": \"string\",\n      \"description\": \"Action to take when a matching alias is found in the target zone. Stop prevents further search rules from being evaluated. Continue allows lower-priority rules to also be evaluated.\",\n      \"enum\": [\"Stop\", \"Continue\"],\n      \"default\": \"Stop\"\n    },\n    \"Description\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Optional description of the search rule's purpose and behavior\",\n      \"maxLength\": 200\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative state of the search rule\",\n      \"enum\": [\"Enabled\", \"Disabled\"],\n      \"default\": \"Enabled\"\n    }\n  },\n  \"required\": [\"Name\", \"AliasPatternType\", \"AliasPatternString\", \"TargetZone\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-search-rule-schema.json
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
