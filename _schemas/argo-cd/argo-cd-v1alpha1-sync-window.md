---
description: v1alpha1SyncWindow schema from Argo CD API
layout: schema
name: v1alpha1SyncWindow
properties_list:
- description: ''
  name: andOperator
  type: boolean
- description: ''
  name: applications
  type: array
- description: ''
  name: clusters
  type: array
- description: ''
  name: description
  type: string
- description: ''
  name: duration
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: manualSync
  type: boolean
- description: ''
  name: namespaces
  type: array
- description: ''
  name: schedule
  type: string
- description: ''
  name: syncOverrun
  type: boolean
- description: ''
  name: timeZone
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-window-schema.json
slug: argo-cd-v1alpha1-sync-window
source_filename: argo-cd-v1alpha1-sync-window-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-window-schema.json\",\n  \"title\": \"v1alpha1SyncWindow\",\n  \"description\": \"v1alpha1SyncWindow schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"andOperator\": {\n      \"type\": \"boolean\",\n      \"title\": \"UseAndOperator use AND operator for matching applications, namespaces and clusters instead of the default OR operator\"\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"title\": \"Applications contains a list of applications that the window will apply to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"clusters\": {\n      \"type\": \"array\",\n      \"title\": \"Clusters contains a list of clusters that the window will apply to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n\
  \    \"description\": {\n      \"type\": \"string\",\n      \"title\": \"Description of the sync that will be applied to the schedule, can be used to add any information such as a ticket number for example\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"title\": \"Duration is the amount of time the sync window will be open\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"title\": \"Kind defines if the window allows or blocks syncs\"\n    },\n    \"manualSync\": {\n      \"type\": \"boolean\",\n      \"title\": \"ManualSync enables manual syncs when they would otherwise be blocked\"\n    },\n    \"namespaces\": {\n      \"type\": \"array\",\n      \"title\": \"Namespaces contains a list of namespaces that the window will apply to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"title\": \"Schedule is the time the window will begin, specified in cron format\"\n    },\n   \
  \ \"syncOverrun\": {\n      \"type\": \"boolean\",\n      \"title\": \"SyncOverrun allows ongoing syncs to continue in two scenarios:\\nFor deny windows: allows syncs that started before the deny window became active to continue running\\nFor allow windows: allows syncs that started during the allow window to continue after the window ends\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"title\": \"TimeZone of the sync that will be applied to the schedule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-window-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncWindow
---
