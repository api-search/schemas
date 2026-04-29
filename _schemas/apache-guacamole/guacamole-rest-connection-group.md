---
description: A group organizing connections and other connection groups
layout: schema
name: ConnectionGroup
properties_list:
- description: Unique group identifier
  name: identifier
  type: string
- description: Group name
  name: name
  type: string
- description: Group type (ORGANIZATIONAL or BALANCING)
  name: type
  type: string
- description: Parent group identifier
  name: parentIdentifier
  type: string
- description: Total active connections in this group
  name: activeConnections
  type: integer
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-connection-group-schema.json
slug: guacamole-rest-connection-group
source_filename: guacamole-rest-connection-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-connection-group-schema.json\",\n  \"title\": \"ConnectionGroup\",\n  \"description\": \"A group organizing connections and other connection groups\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique group identifier\",\n      \"example\": \"1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Group name\",\n      \"example\": \"Production Servers\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Group type (ORGANIZATIONAL or BALANCING)\",\n      \"enum\": [\n        \"ORGANIZATIONAL\",\n        \"BALANCING\"\n      ],\n      \"example\": \"ORGANIZATIONAL\"\n    },\n    \"parentIdentifier\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Parent group identifier\",\n      \"example\": \"ROOT\"\n    },\n    \"activeConnections\": {\n      \"type\": \"integer\",\n      \"description\": \"Total active connections in this group\",\n      \"example\": \"3\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-connection-group-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: ConnectionGroup
---
