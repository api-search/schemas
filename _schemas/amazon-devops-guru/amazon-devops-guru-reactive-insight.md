---
description: Information about a reactive insight. This object is returned by ListInsights.
layout: schema
name: ReactiveInsight
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: InsightTimeRange
  type: object
- description: ''
  name: ResourceCollection
  type: object
- description: ''
  name: SsmOpsItemId
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-reactive-insight-schema.json
slug: amazon-devops-guru-reactive-insight
source_filename: amazon-devops-guru-reactive-insight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-reactive-insight-schema.json\",\n  \"title\": \"ReactiveInsight\",\n  \"description\": \"Information about a reactive insight. This object is returned by ListInsights.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \" The ID of a reactive insight. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightName\"\n        },\n        {\n          \"description\": \" The name of a reactive insight. \"\n        }\n      ]\n    },\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightSeverity\"\n        },\n      \
  \  {\n          \"description\": \"The severity of the insight. For more information, see <a href=\\\"https://docs.aws.amazon.com/devops-guru/latest/userguide/working-with-insights.html#understanding-insights-severities\\\">Understanding insight severities</a> in the <i>Amazon DevOps Guru User Guide</i>.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightStatus\"\n        },\n        {\n          \"description\": \" The status of a reactive insight. \"\n        }\n      ]\n    },\n    \"InsightTimeRange\": {\n      \"$ref\": \"#/components/schemas/InsightTimeRange\"\n    },\n    \"ResourceCollection\": {\n      \"$ref\": \"#/components/schemas/ResourceCollection\"\n    },\n    \"SsmOpsItemId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsmOpsItemId\"\n        },\n        {\n          \"description\": \" The ID of the Amazon Web Services System Manager OpsItem created for this\
  \ insight. You must enable the creation of OpstItems insights before they are created for each insight. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightDescription\"\n        },\n        {\n          \"description\": \"Describes the reactive insight.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-reactive-insight-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: ReactiveInsight
---
