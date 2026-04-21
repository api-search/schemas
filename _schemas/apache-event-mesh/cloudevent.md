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
