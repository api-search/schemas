---
description: <p>A segment from a trace that has been ingested by the X-Ray service. The segment can be compiled from documents uploaded with <a href="https://docs.aws.amazon.com/xray/latest/api/API_PutTraceSegments.html">PutTraceSegments</a>, or an <code>inferred</code> segment for a downstream service, generated from a subsegment sent by the service that called it.</p> <p>For the full segment document schema, see <a href="https://docs.aws.amazon.com/xray/latest/devguide/xray-api-segmentdocuments.html">Amazon Web Services X-Ray Segment Documents</a> in the <i>Amazon Web Services X-Ray Developer Guide</i>.</p>
layout: schema
name: Segment
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Document
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-segment-schema.json
slug: xray-segment
source_filename: xray-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentId\"\n        },\n        {\n          \"description\": \"The segment's ID.\"\n        }\n      ]\n    },\n    \"Document\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentDocument\"\n        },\n        {\n          \"description\": \"The segment document.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>A segment from a trace that has been ingested by the X-Ray service. The segment can be compiled from documents uploaded with <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_PutTraceSegments.html\\\">PutTraceSegments</a>, or an <code>inferred</code> segment for a downstream service, generated from a subsegment sent by the service that called it.</p> <p>For the full segment document schema, see <a href=\\\"https://docs.aws.amazon.com/xray/latest/devguide/xray-api-segmentdocuments.html\\\
  \">Amazon Web Services X-Ray Segment Documents</a> in the <i>Amazon Web Services X-Ray Developer Guide</i>.</p>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Segment\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-segment-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-segment-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Segment
---
