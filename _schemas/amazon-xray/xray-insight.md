---
description: When fault rates go outside of the expected range, X-Ray creates an insight. Insights tracks emergent issues within your applications.
layout: schema
name: Insight
properties_list:
- description: ''
  name: InsightId
  type: object
- description: ''
  name: GroupARN
  type: object
- description: ''
  name: GroupName
  type: object
- description: ''
  name: RootCauseServiceId
  type: object
- description: ''
  name: Categories
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
  name: Summary
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
schema_file: json-schema/xray-insight-schema.json
slug: xray-insight
source_filename: xray-insight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsightId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \"The insights unique identifier. \"\n        }\n      ]\n    },\n    \"GroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the group that the insight belongs to.\"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The name of the group that the insight belongs to.\"\n        }\n      ]\n    },\n    \"RootCauseServiceId\": {\n      \"$ref\": \"#/components/schemas/ServiceId\"\n    },\n    \"Categories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightCategoryList\"\
  \n        },\n        {\n          \"description\": \"The categories that label and describe the type of insight.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightState\"\n        },\n        {\n          \"description\": \"The current state of the insight.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time, in Unix seconds, at which the insight began.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time, in Unix seconds, at which the insight ended.\"\n        }\n      ]\n    },\n    \"Summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightSummaryText\"\n        },\n        {\n\
  \          \"description\": \"A brief description of the insight.\"\n        }\n      ]\n    },\n    \"ClientRequestImpactStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestImpactStatistics\"\n        },\n        {\n          \"description\": \"The impact statistics of the client side service. This includes the number of requests to the client service and whether the requests were faults or okay.\"\n        }\n      ]\n    },\n    \"RootCauseServiceRequestImpactStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestImpactStatistics\"\n        },\n        {\n          \"description\": \"The impact statistics of the root cause service. This includes the number of requests to the client service and whether the requests were faults or okay.\"\n        }\n      ]\n    },\n    \"TopAnomalousServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalousServiceList\"\n\
  \        },\n        {\n          \"description\": \"The service within the insight that is most impacted by the incident.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"When fault rates go outside of the expected range, X-Ray creates an insight. Insights tracks emergent issues within your applications.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Insight\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Insight
---
