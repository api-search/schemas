---
description: An Amazon CloudWatch log group that contains log anomalies and is used to generate an insight.
layout: schema
name: AnomalousLogGroup
properties_list:
- description: ''
  name: LogGroupName
  type: object
- description: ''
  name: ImpactStartTime
  type: object
- description: ''
  name: ImpactEndTime
  type: object
- description: ''
  name: NumberOfLogLinesScanned
  type: object
- description: ''
  name: LogAnomalyShowcases
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-anomalous-log-group-schema.json
slug: amazon-devops-guru-anomalous-log-group
source_filename: amazon-devops-guru-anomalous-log-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-anomalous-log-group-schema.json\",\n  \"title\": \"AnomalousLogGroup\",\n  \"description\": \"An Amazon CloudWatch log group that contains log anomalies and is used to generate an insight.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupName\"\n        },\n        {\n          \"description\": \" The name of the CloudWatch log group. \"\n        }\n      ]\n    },\n    \"ImpactStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The time the anomalous log events began. The impact start time indicates the time of the first log anomaly event that occurs. \"\n        }\n    \
  \  ]\n    },\n    \"ImpactEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The time the anomalous log events stopped. \"\n        }\n      ]\n    },\n    \"NumberOfLogLinesScanned\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfLogLinesScanned\"\n        },\n        {\n          \"description\": \" The number of log lines that were scanned for anomalous log events. \"\n        }\n      ]\n    },\n    \"LogAnomalyShowcases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogAnomalyShowcases\"\n        },\n        {\n          \"description\": \" The log anomalies in the log group. Each log anomaly displayed represents a cluster of similar anomalous log events. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-anomalous-log-group-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: AnomalousLogGroup
---
