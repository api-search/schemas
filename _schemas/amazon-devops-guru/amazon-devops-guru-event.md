---
description: An Amazon Web Services resource event. Amazon Web Services resource events and metrics are analyzed by DevOps Guru to find anomalous behavior and provide recommendations to improve your operational solutions.
layout: schema
name: Event
properties_list:
- description: ''
  name: ResourceCollection
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Time
  type: object
- description: ''
  name: EventSource
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: DataSource
  type: object
- description: ''
  name: EventClass
  type: object
- description: ''
  name: Resources
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-event-schema.json
slug: amazon-devops-guru-event
source_filename: amazon-devops-guru-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"An Amazon Web Services resource event. Amazon Web Services resource events and metrics are analyzed by DevOps Guru to find anomalous behavior and provide recommendations to improve your operational solutions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceCollection\": {\n      \"$ref\": \"#/components/schemas/ResourceCollection\"\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \" The ID of the event. \"\n        }\n      ]\n    },\n    \"Time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" A\
  \ <code>Timestamp</code> that specifies the time the event occurred. \"\n        }\n      ]\n    },\n    \"EventSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventSource\"\n        },\n        {\n          \"description\": \" The Amazon Web Services source that emitted the event. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventName\"\n        },\n        {\n          \"description\": \" The name of the event. \"\n        }\n      ]\n    },\n    \"DataSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventDataSource\"\n        },\n        {\n          \"description\": \" The source, <code>AWS_CLOUD_TRAIL</code> or <code>AWS_CODE_DEPLOY</code>, where DevOps Guru analysis found the event. \"\n        }\n      ]\n    },\n    \"EventClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventClass\"\n   \
  \     },\n        {\n          \"description\": \" The class of the event. The class specifies what the event is related to, such as an infrastructure change, a deployment, or a schema change. \"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventResources\"\n        },\n        {\n          \"description\": \" An <code>EventResource</code> object that contains information about the resource that emitted the event. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-event-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: Event
---
