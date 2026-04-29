---
description: OSSLifecycleRule specifies how to manage bucket's lifecycle
layout: schema
name: io.argoproj.workflow.v1alpha1.OSSLifecycleRule
properties_list:
- description: MarkDeletionAfterDays is the number of days before we delete objects in the bucket
  name: markDeletionAfterDays
  type: integer
- description: MarkInfrequentAccessAfterDays is the number of days before we convert the objects in the bucket to Infrequent Access (IA) storage type
  name: markInfrequentAccessAfterDays
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.OSSLifecycleRule\",\n  \"description\": \"OSSLifecycleRule specifies how to manage bucket's lifecycle\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"markDeletionAfterDays\": {\n      \"description\": \"MarkDeletionAfterDays is the number of days before we delete objects in the bucket\",\n      \"type\": \"integer\"\n    },\n    \"markInfrequentAccessAfterDays\": {\n      \"description\": \"MarkInfrequentAccessAfterDays is the number of days before we convert the objects in the bucket to Infrequent Access (IA) storage type\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.OSSLifecycleRule
---
