---
description: Information about an application that processed requests, users that made requests, or downstream services, resources, and applications that an application used.
layout: schema
name: Service
properties_list:
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Names
  type: object
- description: ''
  name: Root
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Edges
  type: object
- description: ''
  name: SummaryStatistics
  type: object
- description: ''
  name: DurationHistogram
  type: object
- description: ''
  name: ResponseTimeHistogram
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-service-schema.json
slug: xray-service
source_filename: xray-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Identifier for the service. Unique within the service map.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The canonical name of the service.\"\n        }\n      ]\n    },\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceNames\"\n        },\n        {\n          \"description\": \"A list of names for the service, including the canonical name.\"\n        }\n      ]\n    },\n    \"Root\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Indicates that the service was the first service\
  \ to process a request.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifier of the Amazon Web Services account in which the service runs.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The type of service.</p> <ul> <li> <p>Amazon Web Services Resource - The type of an Amazon Web Services resource. For example, <code>AWS::EC2::Instance</code> for an application running on Amazon EC2 or <code>AWS::DynamoDB::Table</code> for an Amazon DynamoDB table that the application used.</p> </li> <li> <p>Amazon Web Services Service - The type of an Amazon Web Services service. For example, <code>AWS::DynamoDB</code> for downstream calls to Amazon DynamoDB that didn't target a specific table.</p> </li> <li> <p> <code>client</code>\
  \ - Represents the clients that sent requests to a root service.</p> </li> <li> <p> <code>remote</code> - A downstream service of indeterminate type.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The service's state.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of the first segment that the service generated.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end time of the last segment that the service generated.\"\n        }\n      ]\n    },\n    \"Edges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EdgeList\"\
  \n        },\n        {\n          \"description\": \"Connections to downstream services.\"\n        }\n      ]\n    },\n    \"SummaryStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceStatistics\"\n        },\n        {\n          \"description\": \"Aggregated statistics for the service.\"\n        }\n      ]\n    },\n    \"DurationHistogram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Histogram\"\n        },\n        {\n          \"description\": \"A histogram that maps the spread of service durations.\"\n        }\n      ]\n    },\n    \"ResponseTimeHistogram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Histogram\"\n        },\n        {\n          \"description\": \"A histogram that maps the spread of service response times.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about an application that processed requests, users that made requests, or\
  \ downstream services, resources, and applications that an application used.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-service-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-service-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Service
---
