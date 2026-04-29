---
description: Subscription schema from Apache EventMesh Admin API
layout: schema
name: Subscription
properties_list:
- description: ''
  name: topic
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: group
  type: string
- description: ''
  name: protocol
  type: string
provider_name: Apache EventMesh
provider_slug: apache-event-mesh
schema_file: json-schema/eventmesh-admin-subscription-schema.json
slug: eventmesh-admin-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-subscription-schema.json\",\n  \"title\": \"Subscription\",\n  \"description\": \"Subscription schema from Apache EventMesh Admin API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"protocol\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-subscription-schema.json
tags:
- Apache
- CloudEvents
- Event-Driven
- Messaging
- Open Source
- Pub-Sub
- Serverless
title: Subscription
---
