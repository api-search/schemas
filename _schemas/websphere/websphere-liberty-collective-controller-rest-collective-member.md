---
description: ''
layout: schema
name: CollectiveMember
properties_list:
- description: Member server name
  name: name
  type: string
- description: Host where the member is located
  name: hostName
  type: string
- description: User directory path
  name: userDir
  type: string
- description: Member status
  name: status
  type: string
- description: Cluster the member belongs to
  name: clusterName
  type: string
- description: HTTPS port
  name: httpsPort
  type: integer
- description: Liberty version
  name: wlpVersion
  type: string
- description: Java version
  name: javaVersion
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-collective-member-schema.json
slug: websphere-liberty-collective-controller-rest-collective-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectiveMember\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Member server name\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Host where the member is located\"\n    },\n    \"userDir\": {\n      \"type\": \"string\",\n      \"description\": \"User directory path\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Member status\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster the member belongs to\"\n    },\n    \"httpsPort\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTPS port\"\n    },\n    \"wlpVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Liberty version\"\n    },\n    \"javaVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Java version\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-collective-member-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: CollectiveMember
---
