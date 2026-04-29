---
description: Describes a related item.
layout: schema
name: ItemValue
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: metricDefinition
  type: object
- description: ''
  name: pagerDutyIncidentDetail
  type: object
- description: ''
  name: url
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-item-value-schema.json
slug: incident-manager-item-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-item-value-schema.json\",\n  \"title\": \"ItemValue\",\n  \"description\": \"Describes a related item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the related item, if the related item is an Amazon resource.\"\n        }\n      ]\n    },\n    \"metricDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDefinition\"\n        },\n        {\n          \"description\": \"The metric definition, if the related item is a metric in Amazon CloudWatch.\"\n        }\n      ]\n    },\n    \"pagerDutyIncidentDetail\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/PagerDutyIncidentDetail\"\n        },\n        {\n          \"description\": \"Details about an incident that is associated with a PagerDuty incident.\"\n        }\n      ]\n    },\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The URL, if the related item is a non-Amazon Web Services resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-item-value-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ItemValue
---
