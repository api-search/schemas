---
description: v1alpha1ApplicationSetStatus schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetStatus
properties_list:
- description: ''
  name: applicationStatus
  type: array
- description: ''
  name: conditions
  type: array
- description: ''
  name: health
  type: object
- description: Resources is a list of Applications resources managed by this application set.
  name: resources
  type: array
- description: ResourcesCount is the total number of resources managed by this application set. The count may be higher than actual number of items in the Resources field when the number of managed resources exceeds
  name: resourcesCount
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-status-schema.json
slug: argo-cd-v1alpha1-application-set-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-status-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetStatus\",\n  \"description\": \"v1alpha1ApplicationSetStatus schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationStatus\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSetApplicationStatus\"\n      }\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"title\": \"INSERT ADDITIONAL STATUS FIELD - define observed state of cluster\\nImportant: Run \\\"make\\\" to regenerate code after modifying this file\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSetCondition\"\n      }\n    },\n    \"health\": {\n      \"$ref\": \"#/definitions/v1alpha1HealthStatus\"\n    },\n    \"resources\"\
  : {\n      \"description\": \"Resources is a list of Applications resources managed by this application set.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/applicationv1alpha1ResourceStatus\"\n      }\n    },\n    \"resourcesCount\": {\n      \"description\": \"ResourcesCount is the total number of resources managed by this application set. The count may be higher than actual number of items in the Resources field when\\nthe number of managed resources exceeds the limit imposed by the controller (to avoid making the status field too large).\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetStatus
---
