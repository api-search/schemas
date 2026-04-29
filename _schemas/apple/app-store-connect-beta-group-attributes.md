---
description: ''
layout: schema
name: BetaGroupAttributes
properties_list:
- description: The name of the beta group
  name: name
  type: string
- description: The date and time the beta group was created
  name: createdDate
  type: string
- description: Whether the group is an internal group
  name: isInternalGroup
  type: boolean
- description: Whether the group has access to all builds
  name: hasAccessToAllBuilds
  type: boolean
- description: Whether the public link is enabled
  name: publicLinkEnabled
  type: boolean
- description: The ID component of the public link
  name: publicLinkId
  type: '[''string'', ''null'']'
- description: The full public TestFlight link
  name: publicLink
  type: '[''string'', ''null'']'
- description: Whether the public link limit is enabled
  name: publicLinkLimitEnabled
  type: boolean
- description: Maximum number of testers via the public link
  name: publicLinkLimit
  type: '[''integer'', ''null'']'
- description: Whether beta feedback is enabled for this group
  name: feedbackEnabled
  type: boolean
- description: Whether iOS builds are available on Apple Silicon Macs
  name: iosBuildsAvailableForAppleSiliconMac
  type: boolean
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-beta-group-attributes-schema.json
slug: app-store-connect-beta-group-attributes
source_filename: app-store-connect-beta-group-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BetaGroupAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the beta group\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the beta group was created\"\n    },\n    \"isInternalGroup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the group is an internal group\"\n    },\n    \"hasAccessToAllBuilds\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the group has access to all builds\"\n    },\n    \"publicLinkEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the public link is enabled\"\n    },\n    \"publicLinkId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The ID component of the public link\"\n    },\n    \"publicLink\": {\n      \"type\": \"['string',\
  \ 'null']\",\n      \"description\": \"The full public TestFlight link\"\n    },\n    \"publicLinkLimitEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the public link limit is enabled\"\n    },\n    \"publicLinkLimit\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Maximum number of testers via the public link\"\n    },\n    \"feedbackEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether beta feedback is enabled for this group\"\n    },\n    \"iosBuildsAvailableForAppleSiliconMac\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether iOS builds are available on Apple Silicon Macs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-beta-group-attributes-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: BetaGroupAttributes
---
