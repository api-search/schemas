---
description: ApplicationSetSyncPolicy configures how generated Applications will relate to their ApplicationSet.
layout: schema
name: v1alpha1ApplicationSetSyncPolicy
properties_list:
- description: ''
  name: applicationsSync
  type: string
- description: PreserveResourcesOnDeletion will preserve resources on deletion. If PreserveResourcesOnDeletion is set to true, these Applications will not be deleted.
  name: preserveResourcesOnDeletion
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-sync-policy-schema.json
slug: argo-cd-v1alpha1-application-set-sync-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-sync-policy-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetSyncPolicy\",\n  \"description\": \"ApplicationSetSyncPolicy configures how generated Applications will relate to their\\nApplicationSet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationsSync\": {\n      \"type\": \"string\",\n      \"title\": \"ApplicationsSync represents the policy applied on the generated applications. Possible values are create-only, create-update, create-delete, sync\\n+kubebuilder:validation:Optional\\n+kubebuilder:validation:Enum=create-only;create-update;create-delete;sync\"\n    },\n    \"preserveResourcesOnDeletion\": {\n      \"description\": \"PreserveResourcesOnDeletion will preserve resources on deletion. If PreserveResourcesOnDeletion is set to true, these Applications\
  \ will not be deleted.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-sync-policy-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetSyncPolicy
---
