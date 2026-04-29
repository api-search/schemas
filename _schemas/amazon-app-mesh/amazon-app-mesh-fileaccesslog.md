---
description: An object that represents an access log file.
layout: schema
name: FileAccessLog
properties_list:
- description: ''
  name: format
  type: object
- description: ''
  name: path
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-fileaccesslog-schema.json
slug: amazon-app-mesh-fileaccesslog
source_filename: amazon-app-mesh-fileaccesslog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FileAccessLog\",\n  \"description\": \"An object that represents an access log file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {},\n    \"path\": {}\n  },\n  \"required\": [\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-fileaccesslog-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: FileAccessLog
---
