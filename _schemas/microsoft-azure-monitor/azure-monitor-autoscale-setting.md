---
description: Represents an Azure Monitor autoscale setting that defines profiles, rules, and capacity limits for automatically scaling Azure resources.
layout: schema
name: Azure Monitor Autoscale Setting
properties_list:
- description: Azure resource ID.
  name: id
  type: string
- description: Azure resource name.
  name: name
  type: string
- description: Azure resource type.
  name: type
  type: string
- description: Resource location.
  name: location
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-autoscale-setting-schema.json
slug: azure-monitor-autoscale-setting
source_filename: azure-monitor-autoscale-setting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/autoscale-setting.json\",\n  \"title\": \"Azure Monitor Autoscale Setting\",\n  \"description\": \"Represents an Azure Monitor autoscale setting that defines profiles, rules, and capacity limits for automatically scaling Azure resources.\",\n  \"type\": \"object\",\n  \"required\": [\"location\", \"properties\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Azure resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Azure resource name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Azure resource type.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Resource location.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n\
  \      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"properties\": {\n      \"$ref\": \"#/$defs/AutoscaleSetting\"\n    }\n  },\n  \"$defs\": {\n    \"AutoscaleSetting\": {\n      \"type\": \"object\",\n      \"required\": [\"profiles\"],\n      \"properties\": {\n        \"profiles\": {\n          \"type\": \"array\",\n          \"maxItems\": 20,\n          \"items\": { \"$ref\": \"#/$defs/AutoscaleProfile\" },\n          \"description\": \"The collection of automatic scaling profiles (maximum 20).\"\n        },\n        \"notifications\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/AutoscaleNotification\" }\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"The enabled flag indicating if autoscale is active.\"\n        },\n        \"predictiveAutoscalePolicy\": {\n          \"$ref\": \"#/$defs/PredictiveAutoscalePolicy\"\n        },\n        \"name\":\
  \ {\n          \"type\": \"string\",\n          \"description\": \"The name of the autoscale setting.\"\n        },\n        \"targetResourceUri\": {\n          \"type\": \"string\",\n          \"description\": \"The resource identifier of the resource that the autoscale setting should be added to.\"\n        },\n        \"targetResourceLocation\": {\n          \"type\": \"string\",\n          \"description\": \"The location of the resource that the autoscale setting should be added to.\"\n        }\n      }\n    },\n    \"AutoscaleProfile\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"capacity\", \"rules\"],\n      \"properties\": {\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the profile.\" },\n        \"capacity\": { \"$ref\": \"#/$defs/ScaleCapacity\" },\n        \"rules\": {\n          \"type\": \"array\",\n          \"maxItems\": 10,\n          \"items\": { \"$ref\": \"#/$defs/ScaleRule\" }\n        },\n        \"fixedDate\": { \"\
  $ref\": \"#/$defs/TimeWindow\" },\n        \"recurrence\": { \"$ref\": \"#/$defs/Recurrence\" }\n      }\n    },\n    \"ScaleCapacity\": {\n      \"type\": \"object\",\n      \"required\": [\"minimum\", \"maximum\", \"default\"],\n      \"properties\": {\n        \"minimum\": { \"type\": \"string\", \"description\": \"The minimum number of instances.\" },\n        \"maximum\": { \"type\": \"string\", \"description\": \"The maximum number of instances.\" },\n        \"default\": { \"type\": \"string\", \"description\": \"The number of instances that will be set if metrics are not available for evaluation.\" }\n      }\n    },\n    \"ScaleRule\": {\n      \"type\": \"object\",\n      \"required\": [\"metricTrigger\", \"scaleAction\"],\n      \"properties\": {\n        \"metricTrigger\": { \"$ref\": \"#/$defs/MetricTrigger\" },\n        \"scaleAction\": { \"$ref\": \"#/$defs/ScaleAction\" }\n      }\n    },\n    \"MetricTrigger\": {\n      \"type\": \"object\",\n      \"required\": [\"metricName\"\
  , \"metricResourceUri\", \"timeGrain\", \"statistic\", \"timeWindow\", \"timeAggregation\", \"operator\", \"threshold\"],\n      \"properties\": {\n        \"metricName\": { \"type\": \"string\" },\n        \"metricNamespace\": { \"type\": \"string\" },\n        \"metricResourceUri\": { \"type\": \"string\" },\n        \"metricResourceLocation\": { \"type\": \"string\" },\n        \"timeGrain\": { \"type\": \"string\" },\n        \"statistic\": { \"type\": \"string\", \"enum\": [\"Average\", \"Min\", \"Max\", \"Sum\"] },\n        \"timeWindow\": { \"type\": \"string\" },\n        \"timeAggregation\": { \"type\": \"string\", \"enum\": [\"Average\", \"Minimum\", \"Maximum\", \"Total\", \"Count\", \"Last\"] },\n        \"operator\": { \"type\": \"string\", \"enum\": [\"Equals\", \"NotEquals\", \"GreaterThan\", \"GreaterThanOrEqual\", \"LessThan\", \"LessThanOrEqual\"] },\n        \"threshold\": { \"type\": \"number\" },\n        \"dividePerInstance\": { \"type\": \"boolean\" }\n      }\n\
  \    },\n    \"ScaleAction\": {\n      \"type\": \"object\",\n      \"required\": [\"direction\", \"type\", \"cooldown\"],\n      \"properties\": {\n        \"direction\": { \"type\": \"string\", \"enum\": [\"None\", \"Increase\", \"Decrease\"] },\n        \"type\": { \"type\": \"string\", \"enum\": [\"ChangeCount\", \"PercentChangeCount\", \"ExactCount\", \"ServiceAllowedNextValue\"] },\n        \"value\": { \"type\": \"string\", \"default\": \"1\" },\n        \"cooldown\": { \"type\": \"string\", \"description\": \"The amount of time to wait since the last scaling action in ISO 8601 duration format.\" }\n      }\n    },\n    \"TimeWindow\": {\n      \"type\": \"object\",\n      \"required\": [\"start\", \"end\"],\n      \"properties\": {\n        \"timeZone\": { \"type\": \"string\" },\n        \"start\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"end\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    },\n    \"Recurrence\": {\n      \"type\": \"\
  object\",\n      \"required\": [\"frequency\", \"schedule\"],\n      \"properties\": {\n        \"frequency\": { \"type\": \"string\", \"enum\": [\"None\", \"Second\", \"Minute\", \"Hour\", \"Day\", \"Week\", \"Month\", \"Year\"] },\n        \"schedule\": { \"$ref\": \"#/$defs/RecurrentSchedule\" }\n      }\n    },\n    \"RecurrentSchedule\": {\n      \"type\": \"object\",\n      \"required\": [\"timeZone\", \"days\", \"hours\", \"minutes\"],\n      \"properties\": {\n        \"timeZone\": { \"type\": \"string\" },\n        \"days\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"hours\": { \"type\": \"array\", \"items\": { \"type\": \"integer\" } },\n        \"minutes\": { \"type\": \"array\", \"items\": { \"type\": \"integer\" } }\n      }\n    },\n    \"AutoscaleNotification\": {\n      \"type\": \"object\",\n      \"required\": [\"operation\"],\n      \"properties\": {\n        \"operation\": { \"type\": \"string\", \"enum\": [\"Scale\"] },\n        \"email\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"sendToSubscriptionAdministrator\": { \"type\": \"boolean\" },\n            \"sendToSubscriptionCoAdministrators\": { \"type\": \"boolean\" },\n            \"customEmails\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          }\n        },\n        \"webhooks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"serviceUri\": { \"type\": \"string\", \"format\": \"uri\" },\n              \"properties\": { \"type\": \"object\", \"additionalProperties\": { \"type\": \"string\" } }\n            }\n          }\n        }\n      }\n    },\n    \"PredictiveAutoscalePolicy\": {\n      \"type\": \"object\",\n      \"required\": [\"scaleMode\"],\n      \"properties\": {\n        \"scaleMode\": { \"type\": \"string\", \"enum\": [\"Disabled\", \"ForecastOnly\", \"Enabled\"] },\n        \"scaleLookAheadTime\": {\
  \ \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-autoscale-setting-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Autoscale Setting
---
