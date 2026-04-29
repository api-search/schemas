---
description: Represents an ephemeral volume that is handled by a normal storage driver.
layout: schema
name: io.k8s.api.core.v1.EphemeralVolumeSource
properties_list:
- description: Will be used to create a stand-alone PVC to provision the volume. The pod in which this EphemeralVolumeSource is embedded will be the owner of the PVC, i.e. the PVC will be deleted together with the p
  name: volumeClaimTemplate
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-ephemeral-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-ephemeral-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-ephemeral-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EphemeralVolumeSource\",\n  \"description\": \"Represents an ephemeral volume that is handled by a normal storage driver.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"volumeClaimTemplate\": {\n      \"description\": \"Will be used to create a stand-alone PVC to provision the volume. The pod in which this EphemeralVolumeSource is embedded will be the owner of the PVC, i.e. the PVC will be deleted together with the pod.  The name of the PVC will be `<pod name>-<volume name>` where `<volume name>` is the name from the `PodSpec.Volumes` array entry. Pod validation will reject the pod if the concatenated name is not valid for a PVC (for example, too long).\\n\\nAn existing PVC with that name\
  \ that is not owned by the pod will *not* be used for the pod to avoid using an unrelated volume by mistake. Starting the pod is then blocked until the unrelated PVC is removed. If such a pre-created PVC is meant to be used by the pod, the PVC has to updated with an owner reference to the pod once the pod exists. Normally this should not be necessary, but it may be useful when manually reconstructing a broken cluster.\\n\\nThis field is read-only and no changes will be made by Kubernetes to the PVC after it has been created.\\n\\nRequired, must not be nil.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PersistentVolumeClaimTemplate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-ephemeral-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EphemeralVolumeSource
---
