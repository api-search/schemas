---
description: Settings for upgrading a cluster.
layout: schema
name: ClusterUpgradeSettings
properties_list:
- description: Settings for overrides during upgrade.
  name: overrideSettings
  type: object
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-cluster-upgrade-settings-schema.json
slug: azure-kubernetes-service-cluster-upgrade-settings
source_filename: azure-kubernetes-service-cluster-upgrade-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterUpgradeSettings\",\n  \"type\": \"object\",\n  \"description\": \"Settings for upgrading a cluster.\",\n  \"properties\": {\n    \"overrideSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for overrides during upgrade.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-cluster-upgrade-settings-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ClusterUpgradeSettings
---
