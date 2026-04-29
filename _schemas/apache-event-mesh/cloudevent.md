---
description: Schema for a CloudEvents v1.0 specification compliant event as used by Apache EventMesh.
layout: schema
name: CloudEvents v1.0
properties_list:
- description: The version of the CloudEvents specification
  name: specversion
  type: string
- description: Identifies the event. Must be unique within the scope of the source.
  name: id
  type: string
- description: Identifies the context in which an event happened
  name: source
  type: string
- description: Describes the type of event related to the originating occurrence
  name: type
  type: string
- description: Content type of the data value (e.g., application/json)
  name: datacontenttype
  type: string
- description: Identifies the schema that data adheres to
  name: dataschema
  type: string
- description: Describes the subject of the event in the context of the event producer
  name: subject
  type: string
- description: Timestamp of when the occurrence happened
  name: time
  type: string
- description: The event payload
  name: data
  type: object
- description: Base64-encoded event payload
  name: data_base64
  type: string
provider_name: Apache EventMesh
provider_slug: apache-event-mesh
schema_file: json-schema/cloudevent.json
slug: cloudevent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/apache-event-mesh/cloudevent.json\",\n  \"title\": \"CloudEvents v1.0\",\n  \"description\": \"Schema for a CloudEvents v1.0 specification compliant event as used by Apache EventMesh.\",\n  \"type\": \"object\",\n  \"required\": [\"specversion\", \"id\", \"source\", \"type\"],\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"const\": \"1.0\",\n      \"description\": \"The version of the CloudEvents specification\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the event. Must be unique within the scope of the source.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"format\": \"uri-reference\",\n      \"description\": \"Identifies the context in which an event happened\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the type\
  \ of event related to the originating occurrence\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\",\n      \"description\": \"Content type of the data value (e.g., application/json)\"\n    },\n    \"dataschema\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Identifies the schema that data adheres to\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the subject of the event in the context of the event producer\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the occurrence happened\"\n    },\n    \"data\": {\n      \"description\": \"The event payload\"\n    },\n    \"data_base64\": {\n      \"type\": \"string\",\n      \"contentEncoding\": \"base64\",\n      \"description\": \"Base64-encoded event payload\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-event-mesh/refs/heads/main/json-schema/cloudevent.json
tags:
- Apache
- CloudEvents
- Event-Driven
- Messaging
- Open Source
- Pub-Sub
- Serverless
title: CloudEvents v1.0
---
