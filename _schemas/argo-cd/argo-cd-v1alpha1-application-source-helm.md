---
description: v1alpha1ApplicationSourceHelm schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourceHelm
properties_list:
- description: APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default, Argo CD uses the API versions of the target cluster. The format is [group/]version/kin
  name: apiVersions
  type: array
- description: ''
  name: fileParameters
  type: array
- description: ''
  name: ignoreMissingValueFiles
  type: boolean
- description: KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD uses the Kubernetes version of the target cluster.
  name: kubeVersion
  type: string
- description: Namespace is an optional namespace to template with. If left empty, defaults to the app's destination namespace.
  name: namespace
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: passCredentials
  type: boolean
- description: ''
  name: releaseName
  type: string
- description: ''
  name: skipCrds
  type: boolean
- description: ''
  name: skipSchemaValidation
  type: boolean
- description: SkipTests skips test manifest installation step (Helm's --skip-tests).
  name: skipTests
  type: boolean
- description: ''
  name: valueFiles
  type: array
- description: ''
  name: values
  type: string
- description: ''
  name: valuesObject
  type: object
- description: ''
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-helm-schema.json
slug: argo-cd-v1alpha1-application-source-helm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-helm-schema.json\",\n  \"title\": \"v1alpha1ApplicationSourceHelm\",\n  \"description\": \"v1alpha1ApplicationSourceHelm schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersions\": {\n      \"description\": \"APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default,\\nArgo CD uses the API versions of the target cluster. The format is [group/]version/kind.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"fileParameters\": {\n      \"type\": \"array\",\n      \"title\": \"FileParameters are file parameters to the helm template\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1HelmFileParameter\"\n      }\n    },\n  \
  \  \"ignoreMissingValueFiles\": {\n      \"type\": \"boolean\",\n      \"title\": \"IgnoreMissingValueFiles prevents helm template from failing when valueFiles do not exist locally by not appending them to helm template --values\"\n    },\n    \"kubeVersion\": {\n      \"description\": \"KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD\\nuses the Kubernetes version of the target cluster.\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace is an optional namespace to template with. If left empty, defaults to the app's destination namespace.\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"Parameters is a list of Helm parameters which are passed to the helm template command upon manifest generation\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1HelmParameter\"\n      }\n    },\n    \"passCredentials\":\
  \ {\n      \"type\": \"boolean\",\n      \"title\": \"PassCredentials pass credentials to all domains (Helm's --pass-credentials)\"\n    },\n    \"releaseName\": {\n      \"type\": \"string\",\n      \"title\": \"ReleaseName is the Helm release name to use. If omitted it will use the application name\"\n    },\n    \"skipCrds\": {\n      \"type\": \"boolean\",\n      \"title\": \"SkipCrds skips custom resource definition installation step (Helm's --skip-crds)\"\n    },\n    \"skipSchemaValidation\": {\n      \"type\": \"boolean\",\n      \"title\": \"SkipSchemaValidation skips JSON schema validation (Helm's --skip-schema-validation)\"\n    },\n    \"skipTests\": {\n      \"description\": \"SkipTests skips test manifest installation step (Helm's --skip-tests).\",\n      \"type\": \"boolean\"\n    },\n    \"valueFiles\": {\n      \"type\": \"array\",\n      \"title\": \"ValuesFiles is a list of Helm value files to use when generating a template\",\n      \"items\": {\n        \"type\": \"\
  string\"\n      }\n    },\n    \"values\": {\n      \"type\": \"string\",\n      \"title\": \"Values specifies Helm values to be passed to helm template, typically defined as a block. ValuesObject takes precedence over Values, so use one or the other.\\n+patchStrategy=replace\"\n    },\n    \"valuesObject\": {\n      \"$ref\": \"#/definitions/runtimeRawExtension\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Version is the Helm version to use for templating (\\\"3\\\")\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-helm-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourceHelm
---
