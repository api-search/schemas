---
description: v1alpha1OrphanedResourcesMonitorSettings schema from Argo CD API
layout: schema
name: v1alpha1OrphanedResourcesMonitorSettings
properties_list:
- description: ''
  name: ignore
  type: array
- description: ''
  name: warn
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-orphaned-resources-monitor-settings-schema.json
slug: argo-cd-v1alpha1-orphaned-resources-monitor-settings
source_filename: argo-cd-v1alpha1-orphaned-resources-monitor-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-orphaned-resources-monitor-settings-schema.json\",\n  \"title\": \"v1alpha1OrphanedResourcesMonitorSettings\",\n  \"description\": \"v1alpha1OrphanedResourcesMonitorSettings schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ignore\": {\n      \"type\": \"array\",\n      \"title\": \"Ignore contains a list of resources that are to be excluded from orphaned resources monitoring\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1OrphanedResourceKey\"\n      }\n    },\n    \"warn\": {\n      \"type\": \"boolean\",\n      \"title\": \"Warn indicates if warning condition should be created for apps which have orphaned resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-orphaned-resources-monitor-settings-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1OrphanedResourcesMonitorSettings
---
