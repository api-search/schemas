---
description: A Scaleway managed Kubernetes cluster (Kapsule or Kosmos)
layout: schema
name: Scaleway Kubernetes Cluster
properties_list:
- description: Unique identifier of the cluster
  name: id
  type: string
- description: Display name of the cluster
  name: name
  type: string
- description: Current status of the cluster
  name: status
  type: string
- description: Kubernetes version running on the cluster
  name: version
  type: string
- description: Region where the cluster is deployed
  name: region
  type: string
- description: Organization ID that owns the cluster
  name: organization_id
  type: string
- description: Project ID the cluster belongs to
  name: project_id
  type: string
- description: User-defined tags for the cluster
  name: tags
  type: array
- description: Container Network Interface plugin used by the cluster
  name: cni
  type: string
- description: Kubernetes API server URL
  name: cluster_url
  type: string
- description: DNS wildcard for node services
  name: dns_wildcard
  type: string
- description: Cluster autoscaler configuration
  name: autoscaler_config
  type: object
- description: Automatic upgrade configuration
  name: auto_upgrade
  type: object
- description: Timestamp when the cluster was created
  name: created_at
  type: string
- description: Timestamp when the cluster was last updated
  name: updated_at
  type: string
provider_name: Scaleway
provider_slug: scaleway
schema_file: json-schema/scaleway-cluster-schema.json
slug: scaleway-cluster
source_filename: scaleway-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scaleway/main/json-schema/scaleway-cluster-schema.json\",\n  \"title\": \"Scaleway Kubernetes Cluster\",\n  \"description\": \"A Scaleway managed Kubernetes cluster (Kapsule or Kosmos)\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\", \"version\", \"region\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the cluster\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the cluster\",\n      \"maxLength\": 100\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown\", \"creating\", \"ready\", \"deleting\", \"deleted\", \"updating\", \"locked\", \"pool_required\", \"warning\"],\n      \"description\": \"Current status of the cluster\"\n    },\n    \"version\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes version running on the cluster\",\n      \"examples\": [\"1.30.0\", \"1.29.3\", \"1.28.5\"]\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region where the cluster is deployed\",\n      \"examples\": [\"fr-par\", \"nl-ams\", \"pl-waw\", \"it-mil\"]\n    },\n    \"organization_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Organization ID that owns the cluster\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Project ID the cluster belongs to\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined tags for the cluster\"\n    },\n    \"cni\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown_cni\", \"cilium\", \"calico\", \"weave\", \"flannel\", \"kilo\"],\n      \"description\"\
  : \"Container Network Interface plugin used by the cluster\"\n    },\n    \"cluster_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Kubernetes API server URL\"\n    },\n    \"dns_wildcard\": {\n      \"type\": \"string\",\n      \"description\": \"DNS wildcard for node services\"\n    },\n    \"autoscaler_config\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster autoscaler configuration\",\n      \"properties\": {\n        \"scale_down_disabled\": {\n          \"type\": \"boolean\"\n        },\n        \"scale_down_delay_after_add\": {\n          \"type\": \"string\"\n        },\n        \"estimator\": {\n          \"type\": \"string\",\n          \"enum\": [\"unknown_estimator\", \"binpacking\"]\n        },\n        \"expander\": {\n          \"type\": \"string\",\n          \"enum\": [\"unknown_expander\", \"random\", \"most_pods\", \"least_waste\", \"priority\", \"price\"]\n        }\n      }\n    },\n    \"auto_upgrade\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Automatic upgrade configuration\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"maintenance_window\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"start_hour\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 23\n            },\n            \"day\": {\n              \"type\": \"string\",\n              \"enum\": [\"any\", \"monday\", \"tuesday\", \"wednesday\", \"thursday\", \"friday\", \"saturday\", \"sunday\"]\n            }\n          }\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cluster was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the cluster was last updated\"\n   \
  \ }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/json-schema/scaleway-cluster-schema.json
tags:
- AI
- Cloud Computing
- Containers
- Database
- European Cloud
- Infrastructure
- Kubernetes
- Serverless
- Storage
title: Scaleway Kubernetes Cluster
---
