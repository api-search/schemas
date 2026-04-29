---
description: Information about a connection between two services. An edge can be a synchronous connection, such as typical call between client and service, or an asynchronous link, such as a Lambda function which retrieves an event from an SNS queue.
layout: schema
name: Edge
properties_list:
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: SummaryStatistics
  type: object
- description: ''
  name: ResponseTimeHistogram
  type: object
- description: ''
  name: Aliases
  type: object
- description: ''
  name: EdgeType
  type: object
- description: ''
  name: ReceivedEventAgeHistogram
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-edge-schema.json
slug: xray-edge
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Identifier of the edge. Unique within a service map.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of the first segment on the edge.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end time of the last segment on the edge.\"\n        }\n      ]\n    },\n    \"SummaryStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EdgeStatistics\"\n        },\n        {\n          \"description\": \"Response statistics for segments on\
  \ the edge.\"\n        }\n      ]\n    },\n    \"ResponseTimeHistogram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Histogram\"\n        },\n        {\n          \"description\": \"A histogram that maps the spread of client response times on an edge. Only populated for synchronous edges.\"\n        }\n      ]\n    },\n    \"Aliases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasList\"\n        },\n        {\n          \"description\": \"Aliases for the edge.\"\n        }\n      ]\n    },\n    \"EdgeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Describes an asynchronous connection, with a value of <code>link</code>.\"\n        }\n      ]\n    },\n    \"ReceivedEventAgeHistogram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Histogram\"\n        },\n        {\n          \"description\"\
  : \"A histogram that maps the spread of event age when received by consumers. Age is calculated each time an event is received. Only populated when <i>EdgeType</i> is <code>link</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about a connection between two services. An edge can be a synchronous connection, such as typical call between client and service, or an asynchronous link, such as a Lambda function which retrieves an event from an SNS queue.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Edge\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-edge-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-edge-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Edge
---
