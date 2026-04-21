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
