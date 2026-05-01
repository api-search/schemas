---
description: Metadata generated from the segment documents in a trace.
layout: schema
name: TraceSummary
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: ResponseTime
  type: object
- description: ''
  name: HasFault
  type: object
- description: ''
  name: HasError
  type: object
- description: ''
  name: HasThrottle
  type: object
- description: ''
  name: IsPartial
  type: object
- description: ''
  name: Http
  type: object
- description: ''
  name: Annotations
  type: object
- description: ''
  name: Users
  type: object
- description: ''
  name: ServiceIds
  type: object
- description: ''
  name: ResourceARNs
  type: object
- description: ''
  name: InstanceIds
  type: object
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: EntryPoint
  type: object
- description: ''
  name: FaultRootCauses
  type: object
- description: ''
  name: ErrorRootCauses
  type: object
- description: ''
  name: ResponseTimeRootCauses
  type: object
- description: ''
  name: Revision
  type: object
- description: ''
  name: MatchedEventTime
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-trace-summary-schema.json
slug: xray-trace-summary
source_filename: xray-trace-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the request that generated the trace's segments and subsegments.\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The length of time in seconds between the start time of the root segment and the end time of the last segment that completed.\"\n        }\n      ]\n    },\n    \"ResponseTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The length of time in seconds between the start and end times of the root segment. If the service performs work asynchronously, the response time measures the time before the\
  \ response is sent to the user, while the duration measures the amount of time before the last traced activity completes.\"\n        }\n      ]\n    },\n    \"HasFault\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"The root segment document has a 500 series error.\"\n        }\n      ]\n    },\n    \"HasError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"The root segment document has a 400 series error.\"\n        }\n      ]\n    },\n    \"HasThrottle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"One or more of the segment documents has a 429 throttling error.\"\n        }\n      ]\n    },\n    \"IsPartial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\
  \n        },\n        {\n          \"description\": \"One or more of the segment documents is in progress.\"\n        }\n      ]\n    },\n    \"Http\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Http\"\n        },\n        {\n          \"description\": \"Information about the HTTP request served by the trace.\"\n        }\n      ]\n    },\n    \"Annotations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Annotations\"\n        },\n        {\n          \"description\": \"Annotations from the trace's segment documents.\"\n        }\n      ]\n    },\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceUsers\"\n        },\n        {\n          \"description\": \"Users from the trace's segment documents.\"\n        }\n      ]\n    },\n    \"ServiceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceIds\"\n        },\n        {\n          \"description\"\
  : \"Service IDs from the trace's segment documents.\"\n        }\n      ]\n    },\n    \"ResourceARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceResourceARNs\"\n        },\n        {\n          \"description\": \"A list of resource ARNs for any resource corresponding to the trace segments.\"\n        }\n      ]\n    },\n    \"InstanceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceInstanceIds\"\n        },\n        {\n          \"description\": \"A list of EC2 instance IDs for any instance corresponding to the trace segments.\"\n        }\n      ]\n    },\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceAvailabilityZones\"\n        },\n        {\n          \"description\": \"A list of Availability Zones for any zone corresponding to the trace segments.\"\n        }\n      ]\n    },\n    \"EntryPoint\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/ServiceId\"\n        },\n        {\n          \"description\": \"The root of a trace.\"\n        }\n      ]\n    },\n    \"FaultRootCauses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FaultRootCauses\"\n        },\n        {\n          \"description\": \"A collection of FaultRootCause structures corresponding to the trace segments.\"\n        }\n      ]\n    },\n    \"ErrorRootCauses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorRootCauses\"\n        },\n        {\n          \"description\": \"A collection of ErrorRootCause structures corresponding to the trace segments.\"\n        }\n      ]\n    },\n    \"ResponseTimeRootCauses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseTimeRootCauses\"\n        },\n        {\n          \"description\": \"A collection of ResponseTimeRootCause structures corresponding to the trace segments.\"\n   \
  \     }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The revision number of a trace.\"\n        }\n      ]\n    },\n    \"MatchedEventTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The matched time stamp of a defined event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Metadata generated from the segment documents in a trace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TraceSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-trace-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-trace-summary-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: TraceSummary
---
