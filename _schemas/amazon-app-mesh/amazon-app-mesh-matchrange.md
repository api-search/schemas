---
description: An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, only values 1-99 would be matched.
layout: schema
name: MatchRange
properties_list:
- description: ''
  name: end
  type: object
- description: ''
  name: start
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-matchrange-schema.json
slug: amazon-app-mesh-matchrange
source_filename: amazon-app-mesh-matchrange-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MatchRange\",\n  \"description\": \"An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, only values 1-99 would be matched.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"end\": {},\n    \"start\": {}\n  },\n  \"required\": [\n    \"end\",\n    \"start\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-matchrange-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: MatchRange
---
