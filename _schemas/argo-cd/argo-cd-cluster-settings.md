---
description: clusterSettings schema from Argo CD API
layout: schema
name: clusterSettings
properties_list:
- description: ''
  name: additionalUrls
  type: array
- description: ''
  name: appLabelKey
  type: string
- description: ''
  name: appsInAnyNamespaceEnabled
  type: boolean
- description: 'Deprecated: use sidecar plugins instead.'
  name: configManagementPlugins
  type: array
- description: ''
  name: controllerNamespace
  type: string
- description: ''
  name: dexConfig
  type: object
- description: ''
  name: execEnabled
  type: boolean
- description: ''
  name: googleAnalytics
  type: object
- description: ''
  name: help
  type: object
- description: ''
  name: hydratorEnabled
  type: boolean
- description: ''
  name: impersonationEnabled
  type: boolean
- description: ''
  name: installationID
  type: string
- description: ''
  name: kustomizeOptions
  type: object
- description: ''
  name: kustomizeVersions
  type: array
- description: ''
  name: oidcConfig
  type: object
- description: ''
  name: passwordPattern
  type: string
- description: ''
  name: plugins
  type: array
- description: ''
  name: resourceOverrides
  type: object
- description: ''
  name: statusBadgeEnabled
  type: boolean
- description: ''
  name: statusBadgeRootUrl
  type: string
- description: ''
  name: syncWithReplaceAllowed
  type: boolean
- description: ''
  name: trackingMethod
  type: string
- description: ''
  name: uiBannerContent
  type: string
- description: ''
  name: uiBannerPermanent
  type: boolean
- description: ''
  name: uiBannerPosition
  type: string
- description: ''
  name: uiBannerURL
  type: string
- description: ''
  name: uiCssURL
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: userLoginsDisabled
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-settings-schema.json
slug: argo-cd-cluster-settings
source_filename: argo-cd-cluster-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-settings-schema.json\",\n  \"title\": \"clusterSettings\",\n  \"description\": \"clusterSettings schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"appLabelKey\": {\n      \"type\": \"string\"\n    },\n    \"appsInAnyNamespaceEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"configManagementPlugins\": {\n      \"description\": \"Deprecated: use sidecar plugins instead.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ConfigManagementPlugin\"\n      }\n    },\n    \"controllerNamespace\": {\n      \"type\": \"string\"\n    },\n    \"dexConfig\": {\n      \"$ref\": \"#/definitions/clusterDexConfig\"\
  \n    },\n    \"execEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"googleAnalytics\": {\n      \"$ref\": \"#/definitions/clusterGoogleAnalyticsConfig\"\n    },\n    \"help\": {\n      \"$ref\": \"#/definitions/clusterHelp\"\n    },\n    \"hydratorEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"impersonationEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"installationID\": {\n      \"type\": \"string\"\n    },\n    \"kustomizeOptions\": {\n      \"$ref\": \"#/definitions/v1alpha1KustomizeOptions\"\n    },\n    \"kustomizeVersions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"oidcConfig\": {\n      \"$ref\": \"#/definitions/clusterOIDCConfig\"\n    },\n    \"passwordPattern\": {\n      \"type\": \"string\"\n    },\n    \"plugins\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/clusterPlugin\"\n      }\n    },\n    \"resourceOverrides\": {\n      \"type\": \"object\"\
  ,\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceOverride\"\n      }\n    },\n    \"statusBadgeEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"statusBadgeRootUrl\": {\n      \"type\": \"string\"\n    },\n    \"syncWithReplaceAllowed\": {\n      \"type\": \"boolean\"\n    },\n    \"trackingMethod\": {\n      \"type\": \"string\"\n    },\n    \"uiBannerContent\": {\n      \"type\": \"string\"\n    },\n    \"uiBannerPermanent\": {\n      \"type\": \"boolean\"\n    },\n    \"uiBannerPosition\": {\n      \"type\": \"string\"\n    },\n    \"uiBannerURL\": {\n      \"type\": \"string\"\n    },\n    \"uiCssURL\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"userLoginsDisabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-settings-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterSettings
---
