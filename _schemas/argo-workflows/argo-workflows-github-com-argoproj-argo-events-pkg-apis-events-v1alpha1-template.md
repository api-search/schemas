---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template
properties_list:
- description: ''
  name: affinity
  type: object
- description: ''
  name: container
  type: object
- description: ''
  name: imagePullSecrets
  type: array
- description: ''
  name: metadata
  type: object
- description: ''
  name: nodeSelector
  type: object
- description: ''
  name: priority
  type: integer
- description: ''
  name: priorityClassName
  type: string
- description: ''
  name: securityContext
  type: object
- description: ''
  name: serviceAccountName
  type: string
- description: ''
  name: tolerations
  type: array
- description: ''
  name: volumes
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-template-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-template
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-template-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"affinity\": {\n      \"title\": \"If specified, the pod's scheduling constraints\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.Affinity\"\n    },\n    \"container\": {\n      \"title\": \"Container is the main container image to run in the sensor pod\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Container\"\n    },\n    \"imagePullSecrets\": {\n      \"type\": \"array\",\n  \
  \    \"title\": \"ImagePullSecrets is an optional list of references to secrets in the same namespace to use for pulling any of the images used by this PodSpec.\\nIf specified, these secrets will be passed to individual puller implementations for them to use. For example,\\nin the case of docker, only DockerConfig type secrets are honored.\\nMore info: https://kubernetes.io/docs/concepts/containers/images#specifying-imagepullsecrets-on-a-pod\\n+optional\\n+patchMergeKey=name\\n+patchStrategy=merge\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n      }\n    },\n    \"metadata\": {\n      \"title\": \"Metadata sets the pods's metadata, i.e. annotations and labels\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Metadata\"\n    },\n    \"nodeSelector\": {\n      \"type\": \"object\",\n      \"title\": \"NodeSelector is a selector which must be true for the pod to fit on a node.\\nSelector which\
  \ must match a node's labels for the pod to be scheduled on that node.\\nMore info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"title\": \"The priority value. Various system components use this field to find the\\npriority of the EventSource pod. When Priority Admission Controller is enabled,\\nit prevents users from setting this field. The admission controller populates\\nthis field from PriorityClassName.\\nThe higher the value, the higher the priority.\\nMore info: https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/\\n+optional\"\n    },\n    \"priorityClassName\": {\n      \"type\": \"string\",\n      \"title\": \"If specified, indicates the EventSource pod's priority. \\\"system-node-critical\\\"\\nand \\\"system-cluster-critical\\\" are two special keywords which indicate the\\nhighest\
  \ priorities with the former being the highest priority. Any other\\nname must be defined by creating a PriorityClass object with that name.\\nIf not specified, the pod priority will be default or zero if there is no\\ndefault.\\nMore info: https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/\\n+optional\"\n    },\n    \"securityContext\": {\n      \"title\": \"SecurityContext holds pod-level security attributes and common container settings.\\nOptional: Defaults to empty.  See type description for default values of each field.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PodSecurityContext\"\n    },\n    \"serviceAccountName\": {\n      \"type\": \"string\",\n      \"title\": \"ServiceAccountName is the name of the ServiceAccount to use to run sensor pod.\\nMore info: https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account/\\n+optional\"\n    },\n    \"tolerations\": {\n      \"type\": \"array\",\n      \"title\":\
  \ \"If specified, the pod's tolerations.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.Toleration\"\n      }\n    },\n    \"volumes\": {\n      \"type\": \"array\",\n      \"title\": \"Volumes is a list of volumes that can be mounted by containers in a io.argoproj.workflow.v1alpha1.\\n+patchStrategy=merge\\n+patchMergeKey=name\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.Volume\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Template
---
