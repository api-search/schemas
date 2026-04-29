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
source_filename: cloudevents-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloudevents.io/schemas/v1/cloudevent.json\",\n  \"title\": \"CloudEvent\",\n  \"description\": \"Schema for a CloudEvents v1.0 event envelope. A CloudEvent is a standardized description of an event produced by a software system. It consists of required context attributes (specversion, id, source, type) and optional context attributes (datacontenttype, dataschema, subject, time), along with an optional data payload. This schema enables consistent event interchange across services, platforms, and cloud providers.\",\n  \"type\": \"object\",\n  \"required\": [\"specversion\", \"id\", \"source\", \"type\"],\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"const\": \"1.0\",\n      \"description\": \"The version of the CloudEvents specification which the event uses. Currently the only supported value is '1.0'.\"\n    },\n    \"id\": {\n      \"type\": \"string\"\
  ,\n      \"minLength\": 1,\n      \"description\": \"Identifies the event. Producers must ensure that source and id together are unique for each distinct event. Consumers may assume that events with identical source and id are duplicates.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"format\": \"uri-reference\",\n      \"description\": \"Identifies the context in which an event happened. Often includes information such as the type of the event source, the organization publishing the event, or the process that produced the event. Must be a non-empty URI-reference.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"This attribute contains a value describing the type of event related to the originating occurrence. Should be prefixed with a reverse-DNS name. The prefixed domain dictates the organization which defines the semantics of this event type.\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Content type of data value. Must adhere to the format specified in RFC 2046. Enables the data attribute to carry any type of content without being limited to JSON.\"\n    },\n    \"dataschema\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Identifies the schema that data adheres to. Incompatible changes to the schema should be reflected by a different URI.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"This describes the subject of the event in the context of the event producer. In publish-subscribe scenarios, a subscriber will typically subscribe to events emitted by a source, but the source identifier alone might not be sufficient as a qualifier for any specific event if the source context has internal sub-structure.\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the occurrence\
  \ happened. If the time of the occurrence cannot be determined, then this attribute may be set to some other time (such as the current time) by the CloudEvents producer.\"\n    },\n    \"data\": {\n      \"description\": \"The event payload. This specification does not place any restriction on the type of this information. It is encoded into a media format which is specified by the datacontenttype attribute.\"\n    },\n    \"data_base64\": {\n      \"type\": \"string\",\n      \"contentEncoding\": \"base64\",\n      \"description\": \"Base64-encoded event payload. This should be used when the data attribute contains binary content that cannot be represented as a UTF-8 string.\"\n    }\n  },\n  \"additionalProperties\": {\n    \"description\": \"CloudEvents extension attributes. Extension attributes are additional metadata beyond the base specification and must use only lowercase letters a-z and digits 0-9 in their names.\"\n  },\n  \"$defs\": {\n    \"CloudEventBatch\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"A batch of CloudEvents serialized as a JSON array. Each element must be a valid CloudEvent. Used in the HTTP structured content mode with application/cloudevents-batch+json media type.\",\n      \"items\": {\n        \"$ref\": \"#\"\n      },\n      \"minItems\": 1\n    },\n    \"DistributedTracingExtension\": {\n      \"type\": \"object\",\n      \"description\": \"CloudEvents Distributed Tracing extension attributes for propagating trace context across event-driven systems. Based on the W3C Trace Context specification.\",\n      \"properties\": {\n        \"traceparent\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9a-f]{2}-[0-9a-f]{32}-[0-9a-f]{16}-[0-9a-f]{2}$\",\n          \"description\": \"W3C Trace Context traceparent header value, encoding version, trace-id, parent-id, and trace-flags.\"\n        },\n        \"tracestate\": {\n          \"type\": \"string\",\n          \"description\": \"W3C Trace Context tracestate header\
  \ value, providing vendor-specific trace information as a comma-separated list of key=value pairs.\"\n        }\n      }\n    },\n    \"PartitioningExtension\": {\n      \"type\": \"object\",\n      \"description\": \"CloudEvents Partitioning extension for directing related events to the same partition in Kafka or similar ordered messaging systems.\",\n      \"properties\": {\n        \"partitionkey\": {\n          \"type\": \"string\",\n          \"description\": \"A partition key that can be used to route events to the same partition in Kafka topics or similar systems, ensuring ordering for related events.\"\n        }\n      }\n    },\n    \"SamplingExtension\": {\n      \"type\": \"object\",\n      \"description\": \"CloudEvents Sampling extension attribute for probabilistic event sampling.\",\n      \"properties\": {\n        \"sampledrate\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Sampled rate as a\
  \ percentage (0-100) indicating what fraction of events from this source are being sent. A value of 100 means all events are sent; 0 means no events are sent.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudevents/refs/heads/main/json-schema/cloudevents-event-schema.json
tags:
- Cloud Native
- Events
- Graduated
- Interoperability
- Messaging
- Specification
title: CloudEvent
---
