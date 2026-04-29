---
description: X-Ray reevaluates insights periodically until they are resolved, and records each intermediate state in an event. You can review incident events in the Impact Timeline on the Inspect page in the X-Ray console.
layout: schema
name: InsightEvent
properties_list:
- description: ''
  name: Summary
  type: object
- description: ''
  name: EventTime
  type: object
- description: ''
  name: ClientRequestImpactStatistics
  type: object
- description: ''
  name: RootCauseServiceRequestImpactStatistics
  type: object
- description: ''
  name: TopAnomalousServices
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-insight-event-schema.json
slug: xray-insight-event
source_filename: xray-insight-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventSummaryText\"\n        },\n        {\n          \"description\": \"A brief description of the event.\"\n        }\n      ]\n    },\n    \"EventTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time, in Unix seconds, at which the event was recorded.\"\n        }\n      ]\n    },\n    \"ClientRequestImpactStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestImpactStatistics\"\n        },\n        {\n          \"description\": \"The impact statistics of the client side service. This includes the number of requests to the client service and whether the requests were faults or okay.\"\n        }\n      ]\n    },\n    \"RootCauseServiceRequestImpactStatistics\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/RequestImpactStatistics\"\n        },\n        {\n          \"description\": \"The impact statistics of the root cause service. This includes the number of requests to the client service and whether the requests were faults or okay.\"\n        }\n      ]\n    },\n    \"TopAnomalousServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalousServiceList\"\n        },\n        {\n          \"description\": \"The service during the event that is most impacted by the incident.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"X-Ray reevaluates insights periodically until they are resolved, and records each intermediate state in an event. You can review incident events in the Impact Timeline on the Inspect page in the X-Ray console.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsightEvent\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-event-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-event-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: InsightEvent
---
