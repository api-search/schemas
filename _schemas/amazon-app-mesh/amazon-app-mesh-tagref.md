---
description: Optional metadata that you apply to a resource to assist with categorization and organization. Each tag consists of a key and an optional value, both of which you define. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.
layout: schema
name: TagRef
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-tagref-schema.json
slug: amazon-app-mesh-tagref
source_filename: amazon-app-mesh-tagref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TagRef\",\n  \"description\": \"Optional metadata that you apply to a resource to assist with categorization and organization. Each tag consists of a key and an optional value, both of which you define. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {},\n    \"value\": {}\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-tagref-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: TagRef
---
