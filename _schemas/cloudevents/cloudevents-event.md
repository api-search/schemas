---
description: Schema for a CloudEvents v1.0 event envelope. A CloudEvent is a standardized description of an event produced by a software system. It consists of required context attributes (specversion, id, source, type) and optional context attributes (datacontenttype, dataschema, subject, time), along with an optional data payload. This schema enables consistent event interchange across services, platforms, and cloud providers.
layout: schema
name: CloudEvent
properties_list:
- description: The version of the CloudEvents specification which the event uses. Currently the only supported value is '1.0'.
  name: specversion
  type: string
- description: Identifies the event. Producers must ensure that source and id together are unique for each distinct event. Consumers may assume that events with identical source and id are duplicates.
  name: id
  type: string
- description: 'Identifies the context in which an event happened. Often includes information such as the type of the event source, the organization publishing the event, or the process that produced the event. Must '
  name: source
  type: string
- description: This attribute contains a value describing the type of event related to the originating occurrence. Should be prefixed with a reverse-DNS name. The prefixed domain dictates the organization which defi
  name: type
  type: string
- description: Content type of data value. Must adhere to the format specified in RFC 2046. Enables the data attribute to carry any type of content without being limited to JSON.
  name: datacontenttype
  type: string
- description: Identifies the schema that data adheres to. Incompatible changes to the schema should be reflected by a different URI.
  name: dataschema
  type: string
- description: This describes the subject of the event in the context of the event producer. In publish-subscribe scenarios, a subscriber will typically subscribe to events emitted by a source, but the source identi
  name: subject
  type: string
- description: Timestamp of when the occurrence happened. If the time of the occurrence cannot be determined, then this attribute may be set to some other time (such as the current time) by the CloudEvents producer.
  name: time
  type: string
- description: The event payload. This specification does not place any restriction on the type of this information. It is encoded into a media format which is specified by the datacontenttype attribute.
  name: data
  type: object
- description: Base64-encoded event payload. This should be used when the data attribute contains binary content that cannot be represented as a UTF-8 string.
  name: data_base64
  type: string
provider_name: CloudEvents
provider_slug: cloudevents
schema_file: json-schema/cloudevents-event-schema.json
slug: cloudevents-event
tags:
- Cloud Native
- Events
- Graduated
- Interoperability
- Messaging
- Specification
title: CloudEvent
---
