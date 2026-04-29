---
description: GeographicSite schema from AT&T API
layout: schema
name: GeographicSite
properties_list:
- description: Unique geographic site identifier
  name: id
  type: string
- description: Name of the geographic site or market area
  name: name
  type: string
- description: URL to this geographic site resource
  name: href
  type: string
- description: Site availability status
  name: status
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-geographic-site-schema.json
slug: mvnx-api-geographic-site
source_filename: mvnx-api-geographic-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-geographic-site-schema.json\",\n  \"title\": \"GeographicSite\",\n  \"description\": \"GeographicSite schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique geographic site identifier\",\n      \"example\": \"site-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the geographic site or market area\",\n      \"example\": \"US Market - East\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to this geographic site resource\",\n      \"example\": \"https://devex-web.att.com/geographicSite/site-500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Site availability status\"\
  ,\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-geographic-site-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: GeographicSite
---
