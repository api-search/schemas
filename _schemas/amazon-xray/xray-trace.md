---
description: A collection of segment documents with matching trace IDs.
layout: schema
name: Trace
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: LimitExceeded
  type: object
- description: ''
  name: Segments
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-trace-schema.json
slug: xray-trace
source_filename: xray-trace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the request that generated the trace's segments and subsegments.\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The length of time in seconds between the start time of the root segment and the end time of the last segment that completed.\"\n        }\n      ]\n    },\n    \"LimitExceeded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"LimitExceeded is set to true when the trace has exceeded the <code>Trace document size</code> limit. For more information about this limit and other X-Ray limits and quotas,\
  \ see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/xray.html\\\">Amazon Web Services X-Ray endpoints and quotas</a>.\"\n        }\n      ]\n    },\n    \"Segments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentList\"\n        },\n        {\n          \"description\": \"Segment documents for the segments and subsegments that comprise the trace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A collection of segment documents with matching trace IDs.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Trace\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-trace-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-trace-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Trace
---
