---
description: Recommendation information to help you remediate detected anomalous behavior that generated an insight.
layout: schema
name: Recommendation
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Link
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Reason
  type: object
- description: ''
  name: RelatedEvents
  type: object
- description: ''
  name: RelatedAnomalies
  type: object
- description: ''
  name: Category
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-recommendation-schema.json
slug: amazon-devops-guru-recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-recommendation-schema.json\",\n  \"title\": \"Recommendation\",\n  \"description\": \"Recommendation information to help you remediate detected anomalous behavior that generated an insight.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationDescription\"\n        },\n        {\n          \"description\": \" A description of the problem. \"\n        }\n      ]\n    },\n    \"Link\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationLink\"\n        },\n        {\n          \"description\": \" A hyperlink to information to help you address the problem. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/RecommendationName\"\n        },\n        {\n          \"description\": \" The name of the recommendation. \"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationReason\"\n        },\n        {\n          \"description\": \" The reason DevOps Guru flagged the anomalous behavior as a problem. \"\n        }\n      ]\n    },\n    \"RelatedEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationRelatedEvents\"\n        },\n        {\n          \"description\": \" Events that are related to the problem. Use these events to learn more about what's happening and to help address the issue. \"\n        }\n      ]\n    },\n    \"RelatedAnomalies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationRelatedAnomalies\"\n        },\n        {\n          \"description\": \" Anomalies that are\
  \ related to the problem. Use these Anomalies to learn more about what's happening and to help address the issue. \"\n        }\n      ]\n    },\n    \"Category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationCategory\"\n        },\n        {\n          \"description\": \"The category type of the recommendation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-recommendation-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: Recommendation
---
