---
description: Operation result from a zone management command
layout: schema
name: Result
properties_list:
- description: Error code if the operation failed
  name: code
  type: string
- description: Human-readable error or status message
  name: message
  type: string
- description: Standard output from the zone administration command
  name: stdout
  type: string
- description: Standard error output from the zone administration command
  name: stderr
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-result-schema.json
slug: solaris-rad-zonemgr-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Result\",\n  \"type\": \"object\",\n  \"description\": \"Operation result from a zone management command\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code if the operation failed\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error or status message\"\n    },\n    \"stdout\": {\n      \"type\": \"string\",\n      \"description\": \"Standard output from the zone administration command\"\n    },\n    \"stderr\": {\n      \"type\": \"string\",\n      \"description\": \"Standard error output from the zone administration command\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-result-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: Result
---
