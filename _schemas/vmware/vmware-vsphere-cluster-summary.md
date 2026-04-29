---
description: Summary of a cluster in the vCenter inventory
layout: schema
name: ClusterSummary
properties_list:
- description: Unique identifier of the cluster (e.g., domain-c7)
  name: cluster
  type: string
- description: Display name of the cluster
  name: name
  type: string
- description: Whether vSphere HA is enabled
  name: ha_enabled
  type: boolean
- description: Whether vSphere DRS is enabled
  name: drs_enabled
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-cluster-summary-schema.json
slug: vmware-vsphere-cluster-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a cluster in the vCenter inventory\",\n  \"properties\": {\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the cluster (e.g., domain-c7)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the cluster\"\n    },\n    \"ha_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether vSphere HA is enabled\"\n    },\n    \"drs_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether vSphere DRS is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-cluster-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: ClusterSummary
---
