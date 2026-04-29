---
description: Details about a reactive anomaly. This object is returned by ListAnomalies.
layout: schema
name: ReactiveAnomaly
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
  name: AnomalyTimeRange
  type: object
- description: ''
  name: AnomalyReportedTimeRange
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
  name: Type
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: CausalAnomalyId
  type: object
- description: ''
  name: AnomalyResources
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-reactive-anomaly-schema.json
slug: amazon-devops-guru-reactive-anomaly
source_filename: amazon-devops-guru-reactive-anomaly-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-reactive-anomaly-schema.json\",\n  \"title\": \"ReactiveAnomaly\",\n  \"description\": \"Details about a reactive anomaly. This object is returned by ListAnomalies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyId\"\n        },\n        {\n          \"description\": \"The ID of the reactive anomaly. \"\n        }\n      ]\n    },\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalySeverity\"\n        },\n        {\n          \"description\": \"The severity of the anomaly. The severity of anomalies that generate an insight determine that insight's severity. For more information, see <a href=\\\"https://docs.aws.amazon.com/devops-guru/latest/userguide/working-with-insights.html#understanding-insights-severities\\\
  \">Understanding insight severities</a> in the <i>Amazon DevOps Guru User Guide</i>.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyStatus\"\n        },\n        {\n          \"description\": \" The status of the anomaly. \"\n        }\n      ]\n    },\n    \"AnomalyTimeRange\": {\n      \"$ref\": \"#/components/schemas/AnomalyTimeRange\"\n    },\n    \"AnomalyReportedTimeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyReportedTimeRange\"\n        },\n        {\n          \"description\": \" An <code>AnomalyReportedTimeRange</code> object that specifies the time range between when the anomaly is opened and the time when it is closed. \"\n        }\n      ]\n    },\n    \"SourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalySourceDetails\"\n        },\n        {\n          \"description\": \" Details about the source\
  \ of the analyzed operational data that triggered the anomaly. The one supported source is Amazon CloudWatch metrics. \"\n        }\n      ]\n    },\n    \"AssociatedInsightId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \" The ID of the insight that contains this anomaly. An insight is composed of related anomalies. \"\n        }\n      ]\n    },\n    \"ResourceCollection\": {\n      \"$ref\": \"#/components/schemas/ResourceCollection\"\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyType\"\n        },\n        {\n          \"description\": \"<p>The type of the reactive anomaly. It can be one of the following types.</p> <ul> <li> <p> <code>CAUSAL</code> - the anomaly can cause a new insight.</p> </li> <li> <p> <code>CONTEXTUAL</code> - the anomaly contains additional information about an insight or its causal anomaly.</p> </li> </ul>\"\
  \n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyName\"\n        },\n        {\n          \"description\": \"The name of the reactive anomaly.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDescription\"\n        },\n        {\n          \"description\": \"A description of the reactive anomaly.\"\n        }\n      ]\n    },\n    \"CausalAnomalyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyId\"\n        },\n        {\n          \"description\": \"The ID of the causal anomaly that is associated with this reactive anomaly. The ID of a `CAUSAL` anomaly is always `NULL`.\"\n        }\n      ]\n    },\n    \"AnomalyResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyResources\"\n        },\n        {\n          \"description\": \"The Amazon\
  \ Web Services resources in which anomalous behavior was detected by DevOps Guru.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-reactive-anomaly-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: ReactiveAnomaly
---
