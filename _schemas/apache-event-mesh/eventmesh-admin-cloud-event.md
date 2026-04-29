---
description: A CloudEvents v1.0 compliant event
layout: schema
name: CloudEvent
properties_list:
- description: CloudEvents specification version
  name: specversion
  type: string
- description: Unique event identifier
  name: id
  type: string
- description: Event source identifier
  name: source
  type: string
- description: Event type
  name: type
  type: string
- description: Content type of the data attribute
  name: datacontenttype
  type: string
- description: Schema for the data attribute
  name: dataschema
  type: string
- description: Subject of the event in the context of the source
  name: subject
  type: string
- description: Timestamp of the event
  name: time
  type: string
- description: Event payload
  name: data
  type: object
- description: Base64 encoded event payload
  name: data_base64
  type: string
provider_name: Apache EventMesh
provider_slug: apache-event-mesh
schema_file: json-schema/eventmesh-admin-cloud-event-schema.json
slug: eventmesh-admin-cloud-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-cloud-event-schema.json\",\n  \"title\": \"CloudEvent\",\n  \"description\": \"A CloudEvents v1.0 compliant event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"const\": \"1.0\",\n      \"description\": \"CloudEvents specification version\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"format\": \"uri-reference\",\n      \"description\": \"Event source identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Event type\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\",\n      \"description\": \"Content type of the data attribute\"\n    },\n    \"dataschema\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Schema for the data attribute\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Subject of the event in the context of the source\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the event\"\n    },\n    \"data\": {\n      \"description\": \"Event payload\"\n    },\n    \"data_base64\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"description\": \"Base64 encoded event payload\"\n    }\n  },\n  \"required\": [\n    \"specversion\",\n    \"id\",\n    \"source\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/eventmesh-admin-cloud-event-schema.json
tags:
- Apache
- CloudEvents
- Event-Driven
- Messaging
- Open Source
- Pub-Sub
- Serverless
title: CloudEvent
---
