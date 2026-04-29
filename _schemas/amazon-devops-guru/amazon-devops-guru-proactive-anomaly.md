---
description: Information about an anomaly. This object is returned by ListAnomalies.
layout: schema
name: ProactiveAnomaly
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: UpdateTime
  type: object
- description: ''
  name: AnomalyTimeRange
  type: object
- description: ''
  name: AnomalyReportedTimeRange
  type: object
- description: ''
  name: PredictionTimeRange
  type: object
- description: ''
  name: SourceDetails
  type: object
- description: ''
  name: AssociatedInsightId
  type: object
- description: ''
  name: ResourceCollection
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: SourceMetadata
  type: object
- description: ''
  name: AnomalyResources
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-proactive-anomaly-schema.json
slug: amazon-devops-guru-proactive-anomaly
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-proactive-anomaly-schema.json\",\n  \"title\": \"ProactiveAnomaly\",\n  \"description\": \"Information about an anomaly. This object is returned by ListAnomalies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyId\"\n        },\n        {\n          \"description\": \" The ID of a proactive anomaly. \"\n        }\n      ]\n    },\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalySeverity\"\n        },\n        {\n          \"description\": \"The severity of the anomaly. The severity of anomalies that generate an insight determine that insight's severity. For more information, see <a href=\\\"https://docs.aws.amazon.com/devops-guru/latest/userguide/working-with-insights.html#understanding-insights-severities\\\
  \">Understanding insight severities</a> in the <i>Amazon DevOps Guru User Guide</i>.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyStatus\"\n        },\n        {\n          \"description\": \" The status of a proactive anomaly. \"\n        }\n      ]\n    },\n    \"UpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The time of the anomaly's most recent update. \"\n        }\n      ]\n    },\n    \"AnomalyTimeRange\": {\n      \"$ref\": \"#/components/schemas/AnomalyTimeRange\"\n    },\n    \"AnomalyReportedTimeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyReportedTimeRange\"\n        },\n        {\n          \"description\": \" An <code>AnomalyReportedTimeRange</code> object that specifies the time range between when the anomaly is opened and the time\
  \ when it is closed. \"\n        }\n      ]\n    },\n    \"PredictionTimeRange\": {\n      \"$ref\": \"#/components/schemas/PredictionTimeRange\"\n    },\n    \"SourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalySourceDetails\"\n        },\n        {\n          \"description\": \" Details about the source of the analyzed operational data that triggered the anomaly. The one supported source is Amazon CloudWatch metrics. \"\n        }\n      ]\n    },\n    \"AssociatedInsightId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \" The ID of the insight that contains this anomaly. An insight is composed of related anomalies. \"\n        }\n      ]\n    },\n    \"ResourceCollection\": {\n      \"$ref\": \"#/components/schemas/ResourceCollection\"\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyLimit\"\
  \n        },\n        {\n          \"description\": \" A threshold that was exceeded by behavior in analyzed resources. Exceeding this threshold is related to the anomalous behavior that generated this anomaly. \"\n        }\n      ]\n    },\n    \"SourceMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalySourceMetadata\"\n        },\n        {\n          \"description\": \"The metadata for the anomaly.\"\n        }\n      ]\n    },\n    \"AnomalyResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyResources\"\n        },\n        {\n          \"description\": \"Information about a resource in which DevOps Guru detected anomalous behavior.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDescription\"\n        },\n        {\n          \"description\": \" A description of the proactive anomaly. \"\n        }\n    \
  \  ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-proactive-anomaly-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: ProactiveAnomaly
---
