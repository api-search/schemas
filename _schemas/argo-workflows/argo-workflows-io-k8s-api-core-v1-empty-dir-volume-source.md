---
description: Represents an empty directory for a pod. Empty directory volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.EmptyDirVolumeSource
properties_list:
- description: 'medium represents what type of storage medium should back this directory. The default is "" which means to use the node''s default medium. Must be an empty string (default) or Memory. More info: https:'
  name: medium
  type: string
- description: 'sizeLimit is the total amount of local storage required for this EmptyDir volume. The size limit is also applicable for memory medium. The maximum usage on memory medium EmptyDir would be the minimum '
  name: sizeLimit
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-empty-dir-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-empty-dir-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-empty-dir-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-empty-dir-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EmptyDirVolumeSource\",\n  \"description\": \"Represents an empty directory for a pod. Empty directory volumes support ownership management and SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"medium\": {\n      \"description\": \"medium represents what type of storage medium should back this directory. The default is \\\"\\\" which means to use the node's default medium. Must be an empty string (default) or Memory. More info: https://kubernetes.io/docs/concepts/storage/volumes#emptydir\",\n      \"type\": \"string\"\n    },\n    \"sizeLimit\": {\n      \"description\": \"sizeLimit is the total amount of local storage required for this EmptyDir volume. The size limit is\
  \ also applicable for memory medium. The maximum usage on memory medium EmptyDir would be the minimum value between the SizeLimit specified here and the sum of memory limits of all containers in a pod. The default is nil which means that the limit is undefined. More info: https://kubernetes.io/docs/concepts/storage/volumes#emptydir\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.api.resource.Quantity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-empty-dir-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EmptyDirVolumeSource
---
