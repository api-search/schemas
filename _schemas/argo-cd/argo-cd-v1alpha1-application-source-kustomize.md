---
description: v1alpha1ApplicationSourceKustomize schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourceKustomize
properties_list:
- description: APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default, Argo CD uses the API versions of the target cluster. The format is [group/]version/kin
  name: apiVersions
  type: array
- description: ''
  name: commonAnnotations
  type: object
- description: ''
  name: commonAnnotationsEnvsubst
  type: boolean
- description: ''
  name: commonLabels
  type: object
- description: ''
  name: components
  type: array
- description: ''
  name: forceCommonAnnotations
  type: boolean
- description: ''
  name: forceCommonLabels
  type: boolean
- description: ''
  name: ignoreMissingComponents
  type: boolean
- description: ''
  name: images
  type: array
- description: KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD uses the Kubernetes version of the target cluster.
  name: kubeVersion
  type: string
- description: ''
  name: labelIncludeTemplates
  type: boolean
- description: ''
  name: labelWithoutSelector
  type: boolean
- description: ''
  name: namePrefix
  type: string
- description: ''
  name: nameSuffix
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: patches
  type: array
- description: ''
  name: replicas
  type: array
- description: ''
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-kustomize-schema.json
slug: argo-cd-v1alpha1-application-source-kustomize
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-kustomize-schema.json\",\n  \"title\": \"v1alpha1ApplicationSourceKustomize\",\n  \"description\": \"v1alpha1ApplicationSourceKustomize schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersions\": {\n      \"description\": \"APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default,\\nArgo CD uses the API versions of the target cluster. The format is [group/]version/kind.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"commonAnnotations\": {\n      \"type\": \"object\",\n      \"title\": \"CommonAnnotations is a list of additional annotations to add to rendered manifests\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\
  \n      }\n    },\n    \"commonAnnotationsEnvsubst\": {\n      \"type\": \"boolean\",\n      \"title\": \"CommonAnnotationsEnvsubst specifies whether to apply env variables substitution for annotation values\"\n    },\n    \"commonLabels\": {\n      \"type\": \"object\",\n      \"title\": \"CommonLabels is a list of additional labels to add to rendered manifests\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"title\": \"Components specifies a list of kustomize components to add to the kustomization before building\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"forceCommonAnnotations\": {\n      \"type\": \"boolean\",\n      \"title\": \"ForceCommonAnnotations specifies whether to force applying common annotations to resources for Kustomize apps\"\n    },\n    \"forceCommonLabels\": {\n      \"type\": \"boolean\",\n      \"title\": \"ForceCommonLabels specifies\
  \ whether to force applying common labels to resources for Kustomize apps\"\n    },\n    \"ignoreMissingComponents\": {\n      \"type\": \"boolean\",\n      \"title\": \"IgnoreMissingComponents prevents kustomize from failing when components do not exist locally by not appending them to kustomization file\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"title\": \"Images is a list of Kustomize image override specifications\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"kubeVersion\": {\n      \"description\": \"KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD\\nuses the Kubernetes version of the target cluster.\",\n      \"type\": \"string\"\n    },\n    \"labelIncludeTemplates\": {\n      \"type\": \"boolean\",\n      \"title\": \"LabelIncludeTemplates specifies whether to apply common labels to resource templates or not\"\n    },\n    \"labelWithoutSelector\": {\n      \"type\"\
  : \"boolean\",\n      \"title\": \"LabelWithoutSelector specifies whether to apply common labels to resource selectors or not\"\n    },\n    \"namePrefix\": {\n      \"type\": \"string\",\n      \"title\": \"NamePrefix overrides the namePrefix in the kustomization.yaml for Kustomize apps\"\n    },\n    \"nameSuffix\": {\n      \"type\": \"string\",\n      \"title\": \"NameSuffix overrides the nameSuffix in the kustomization.yaml for Kustomize apps\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"title\": \"Namespace sets the namespace that Kustomize adds to all resources\"\n    },\n    \"patches\": {\n      \"type\": \"array\",\n      \"title\": \"Patches is a list of Kustomize patches\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1KustomizePatch\"\n      }\n    },\n    \"replicas\": {\n      \"type\": \"array\",\n      \"title\": \"Replicas is a list of Kustomize Replicas override specifications\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1KustomizeReplica\"\
  \n      }\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Version controls which version of Kustomize to use for rendering manifests\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-kustomize-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourceKustomize
---
