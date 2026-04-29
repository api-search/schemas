---
description: A Workload Domain represents a logically isolated group of clusters in VMware Cloud Foundation that provides compute, storage, and networking resources for a specific workload type.
layout: schema
name: Broadcom Workload Domain
properties_list:
- description: The unique identifier of the workload domain.
  name: id
  type: string
- description: The name of the workload domain.
  name: name
  type: string
- description: The type of workload domain. MANAGEMENT is the initial domain, VI is a Virtual Infrastructure domain.
  name: type
  type: string
- description: The current status of the workload domain.
  name: status
  type: string
- description: The clusters that belong to this workload domain.
  name: clusters
  type: array
- description: The SSO domain identifier associated with this workload domain.
  name: ssoId
  type: string
- description: The vCenter Server associated with this workload domain.
  name: vcenter
  type: object
- description: The NSX-T cluster associated with this workload domain.
  name: nsxTCluster
  type: object
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-workload-domain-schema.json
slug: broadcom-workload-domain
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-workload-domain-schema.json\",\n  \"title\": \"Broadcom Workload Domain\",\n  \"description\": \"A Workload Domain represents a logically isolated group of clusters in VMware Cloud Foundation that provides compute, storage, and networking resources for a specific workload type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workload domain.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workload domain.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MANAGEMENT\",\n        \"VI\"\n      ],\n      \"description\": \"The type of workload domain. MANAGEMENT is the initial domain, VI is a Virtual Infrastructure domain.\"\n    },\n    \"status\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ERROR\",\n        \"ACTIVATING\",\n        \"DELETING\"\n      ],\n      \"description\": \"The current status of the workload domain.\"\n    },\n    \"clusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The identifier of the cluster.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the cluster.\"\n          },\n          \"primaryDatastoreType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"VSAN\",\n              \"VMFS_FC\",\n              \"VMFS_ISCSI\",\n              \"NFS\",\n              \"VVOL\"\n            ],\n            \"description\": \"The primary datastore type of the cluster.\"\n          },\n          \"isDefault\": {\n          \
  \  \"type\": \"boolean\",\n            \"description\": \"Whether this is the default cluster in the domain.\"\n          },\n          \"hosts\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\",\n                  \"description\": \"The identifier of the host.\"\n                },\n                \"fqdn\": {\n                  \"type\": \"string\",\n                  \"description\": \"The fully qualified domain name of the host.\"\n                }\n              }\n            },\n            \"description\": \"The hosts in the cluster.\"\n          }\n        }\n      },\n      \"description\": \"The clusters that belong to this workload domain.\"\n    },\n    \"ssoId\": {\n      \"type\": \"string\",\n      \"description\": \"The SSO domain identifier associated with this workload domain.\"\n    },\n    \"vcenter\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"The vCenter Server associated with this workload domain.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the vCenter.\"\n        },\n        \"fqdn\": {\n          \"type\": \"string\",\n          \"description\": \"The fully qualified domain name of the vCenter.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of vCenter Server.\"\n        }\n      }\n    },\n    \"nsxTCluster\": {\n      \"type\": \"object\",\n      \"description\": \"The NSX-T cluster associated with this workload domain.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the NSX-T cluster.\"\n        },\n        \"vip\": {\n          \"type\": \"string\",\n          \"description\": \"The virtual IP address of the NSX-T cluster.\"\n        }\n      }\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-workload-domain-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Workload Domain
---
