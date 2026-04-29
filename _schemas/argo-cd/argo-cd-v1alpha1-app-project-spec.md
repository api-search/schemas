---
description: v1alpha1AppProjectSpec schema from Argo CD API
layout: schema
name: v1alpha1AppProjectSpec
properties_list:
- description: ''
  name: clusterResourceBlacklist
  type: array
- description: ''
  name: clusterResourceWhitelist
  type: array
- description: ''
  name: description
  type: string
- description: DestinationServiceAccounts holds information about the service accounts to be impersonated for the application sync operation for each destination.
  name: destinationServiceAccounts
  type: array
- description: ''
  name: destinations
  type: array
- description: ''
  name: namespaceResourceBlacklist
  type: array
- description: ''
  name: namespaceResourceWhitelist
  type: array
- description: ''
  name: orphanedResources
  type: object
- description: ''
  name: permitOnlyProjectScopedClusters
  type: boolean
- description: ''
  name: roles
  type: array
- description: ''
  name: signatureKeys
  type: array
- description: ''
  name: sourceNamespaces
  type: array
- description: ''
  name: sourceRepos
  type: array
- description: ''
  name: syncWindows
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-app-project-spec-schema.json
slug: argo-cd-v1alpha1-app-project-spec
source_filename: argo-cd-v1alpha1-app-project-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-spec-schema.json\",\n  \"title\": \"v1alpha1AppProjectSpec\",\n  \"description\": \"v1alpha1AppProjectSpec schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterResourceBlacklist\": {\n      \"type\": \"array\",\n      \"title\": \"ClusterResourceBlacklist contains list of blacklisted cluster level resources\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ClusterResourceRestrictionItem\"\n      }\n    },\n    \"clusterResourceWhitelist\": {\n      \"type\": \"array\",\n      \"title\": \"ClusterResourceWhitelist contains list of whitelisted cluster level resources\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ClusterResourceRestrictionItem\"\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n\
  \      \"title\": \"Description contains optional project description\\n+kubebuilder:validation:MaxLength=255\"\n    },\n    \"destinationServiceAccounts\": {\n      \"description\": \"DestinationServiceAccounts holds information about the service accounts to be impersonated for the application sync operation for each destination.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationDestinationServiceAccount\"\n      }\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"title\": \"Destinations contains list of destinations available for deployment\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationDestination\"\n      }\n    },\n    \"namespaceResourceBlacklist\": {\n      \"type\": \"array\",\n      \"title\": \"NamespaceResourceBlacklist contains list of blacklisted namespace level resources\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1GroupKind\"\n      }\n    },\n    \"namespaceResourceWhitelist\"\
  : {\n      \"type\": \"array\",\n      \"title\": \"NamespaceResourceWhitelist contains list of whitelisted namespace level resources\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1GroupKind\"\n      }\n    },\n    \"orphanedResources\": {\n      \"$ref\": \"#/definitions/v1alpha1OrphanedResourcesMonitorSettings\"\n    },\n    \"permitOnlyProjectScopedClusters\": {\n      \"type\": \"boolean\",\n      \"title\": \"PermitOnlyProjectScopedClusters determines whether destinations can only reference clusters which are project-scoped\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"title\": \"Roles are user defined RBAC roles associated with this project\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ProjectRole\"\n      }\n    },\n    \"signatureKeys\": {\n      \"type\": \"array\",\n      \"title\": \"SignatureKeys contains a list of PGP key IDs that commits in Git must be signed with in order to be allowed for sync\",\n      \"items\": {\n\
  \        \"$ref\": \"#/definitions/v1alpha1SignatureKey\"\n      }\n    },\n    \"sourceNamespaces\": {\n      \"type\": \"array\",\n      \"title\": \"SourceNamespaces defines the namespaces application resources are allowed to be created in\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sourceRepos\": {\n      \"type\": \"array\",\n      \"title\": \"SourceRepos contains list of repository URLs which can be used for deployment\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"syncWindows\": {\n      \"type\": \"array\",\n      \"title\": \"SyncWindows controls when syncs can be run for apps in this project\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1SyncWindow\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-app-project-spec-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1AppProjectSpec
---
