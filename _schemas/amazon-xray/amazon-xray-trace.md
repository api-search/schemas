---
description: Schema representing an AWS X-Ray trace resource for distributed tracing.
layout: schema
name: AWS X-Ray Trace
properties_list:
- description: The unique identifier for the request trace.
  name: Id
  type: string
- description: The length of time in seconds between the start and end of the trace.
  name: Duration
  type: number
- description: Whether the trace exceeded the segment document size limit.
  name: LimitExceeded
  type: boolean
- description: The segment documents associated with the trace.
  name: Segments
  type: array
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/amazon-xray-trace-schema.json
slug: amazon-xray-trace
source_filename: amazon-xray-trace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://xray.amazonaws.com/schemas/trace\",\n  \"title\": \"AWS X-Ray Trace\",\n  \"description\": \"Schema representing an AWS X-Ray trace resource for distributed tracing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the request trace.\",\n      \"pattern\": \"^1-[0-9a-f]{8}-[0-9a-f]{24}$\"\n    },\n    \"Duration\": {\n      \"type\": \"number\",\n      \"description\": \"The length of time in seconds between the start and end of the trace.\"\n    },\n    \"LimitExceeded\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the trace exceeded the segment document size limit.\"\n    },\n    \"Segments\": {\n      \"type\": \"array\",\n      \"description\": \"The segment documents associated with the trace.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Segment\"\n      }\n\
  \    }\n  },\n  \"$defs\": {\n    \"Segment\": {\n      \"type\": \"object\",\n      \"description\": \"A segment document representing a unit of work in the trace.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"The segment ID.\",\n          \"pattern\": \"^[0-9a-f]{16}$\"\n        },\n        \"Document\": {\n          \"type\": \"string\",\n          \"description\": \"The segment document as a JSON string.\"\n        }\n      }\n    },\n    \"SegmentDocument\": {\n      \"type\": \"object\",\n      \"description\": \"The parsed content of a segment document.\",\n      \"required\": [\n        \"name\",\n        \"id\",\n        \"trace_id\",\n        \"start_time\",\n        \"end_time\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The logical name of the service.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"A 64-bit identifier for the segment.\"\n        },\n        \"trace_id\": {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier that connects segments for a single request.\"\n        },\n        \"start_time\": {\n          \"type\": \"number\",\n          \"description\": \"The time the segment was created, in epoch seconds.\"\n        },\n        \"end_time\": {\n          \"type\": \"number\",\n          \"description\": \"The time the segment was closed, in epoch seconds.\"\n        },\n        \"in_progress\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the segment is in progress.\"\n        },\n        \"http\": {\n          \"type\": \"object\",\n          \"description\": \"HTTP request and response information.\",\n          \"properties\": {\n            \"request\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"method\": {\n                  \"type\": \"string\"\n \
  \               },\n                \"url\": {\n                  \"type\": \"string\"\n                },\n                \"client_ip\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"response\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"status\": {\n                  \"type\": \"integer\"\n                },\n                \"content_length\": {\n                  \"type\": \"integer\"\n                }\n              }\n            }\n          }\n        },\n        \"fault\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the segment recorded a fault (5xx error).\"\n        },\n        \"error\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the segment recorded an error (4xx error).\"\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value pairs for filtering\
  \ traces.\",\n          \"additionalProperties\": true\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Object with any keys and values for storing trace data.\",\n          \"additionalProperties\": true\n        },\n        \"subsegments\": {\n          \"type\": \"array\",\n          \"description\": \"Subsegments representing downstream calls.\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/amazon-xray-trace-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: AWS X-Ray Trace
---
