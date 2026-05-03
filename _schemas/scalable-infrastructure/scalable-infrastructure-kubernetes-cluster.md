---
description: Describes a managed Kubernetes cluster configuration across AWS EKS, Google GKE, Azure AKS, and DigitalOcean DOKS. Covers node pools, networking, autoscaling, and access control.
layout: schema
name: Kubernetes Cluster
properties_list:
- description: Provider-assigned unique cluster identifier.
  name: id
  type: string
- description: Human-readable cluster name.
  name: name
  type: string
- description: Cloud provider hosting the managed Kubernetes cluster.
  name: provider
  type: string
- description: Cloud region where the cluster control plane resides.
  name: region
  type: string
- description: Kubernetes version (e.g., 1.29, 1.30).
  name: version
  type: string
- description: Current operational status of the cluster.
  name: status
  type: string
- description: API server endpoint URL for kubectl and client access.
  name: endpoint
  type: string
- description: Node pools (worker node groups) in the cluster.
  name: nodePools
  type: array
- description: ''
  name: networking
  type: object
- description: ''
  name: autoscaling
  type: object
- description: Managed cluster add-ons or extensions enabled.
  name: addons
  type: array
- description: Key-value metadata labels.
  name: tags
  type: object
- description: Cluster creation timestamp.
  name: createdAt
  type: string
provider_name: Scalable Infrastructure
provider_slug: scalable-infrastructure
schema_file: json-schema/scalable-infrastructure-kubernetes-cluster-schema.json
slug: scalable-infrastructure-kubernetes-cluster
source_filename: scalable-infrastructure-kubernetes-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/main/json-schema/scalable-infrastructure-kubernetes-cluster-schema.json\",\n  \"title\": \"Kubernetes Cluster\",\n  \"description\": \"Describes a managed Kubernetes cluster configuration across AWS EKS, Google GKE, Azure AKS, and DigitalOcean DOKS. Covers node pools, networking, autoscaling, and access control.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"provider\", \"region\", \"version\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Provider-assigned unique cluster identifier.\",\n      \"example\": \"cluster-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable cluster name.\",\n      \"pattern\": \"^[a-z][a-z0-9-]*$\",\n      \"minLength\": 1,\n      \"maxLength\": 63\n    },\n    \"provider\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Cloud provider hosting the managed Kubernetes cluster.\",\n      \"enum\": [\"aws-eks\", \"google-gke\", \"azure-aks\", \"digitalocean-doks\", \"self-managed\"]\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where the cluster control plane resides.\",\n      \"examples\": [\"us-east-1\", \"us-central1\", \"eastus\", \"nyc3\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes version (e.g., 1.29, 1.30).\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+(\\\\.\\\\d+)?$\",\n      \"example\": \"1.30\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the cluster.\",\n      \"enum\": [\"provisioning\", \"running\", \"upgrading\", \"degraded\", \"deleting\", \"deleted\"],\n      \"default\": \"provisioning\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"API server endpoint\
  \ URL for kubectl and client access.\",\n      \"format\": \"uri\"\n    },\n    \"nodePools\": {\n      \"type\": \"array\",\n      \"description\": \"Node pools (worker node groups) in the cluster.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/NodePool\"\n      }\n    },\n    \"networking\": {\n      \"$ref\": \"#/$defs/ClusterNetworking\"\n    },\n    \"autoscaling\": {\n      \"$ref\": \"#/$defs/ClusterAutoscaling\"\n    },\n    \"addons\": {\n      \"type\": \"array\",\n      \"description\": \"Managed cluster add-ons or extensions enabled.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"name\"],\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"examples\": [\"coredns\", \"kube-proxy\", \"vpc-cni\", \"metrics-server\", \"cluster-autoscaler\"]\n          },\n          \"version\": {\"type\": \"string\"},\n          \"enabled\": {\"type\": \"boolean\", \"default\": true}\n\
  \        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value metadata labels.\",\n      \"additionalProperties\": {\"type\": \"string\"}\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Cluster creation timestamp.\"\n    }\n  },\n  \"$defs\": {\n    \"NodePool\": {\n      \"type\": \"object\",\n      \"description\": \"A pool of homogeneous worker nodes with shared configuration.\",\n      \"required\": [\"name\", \"instanceType\", \"minCount\", \"maxCount\"],\n      \"properties\": {\n        \"name\": {\"type\": \"string\", \"description\": \"Node pool name.\"},\n        \"instanceType\": {\n          \"type\": \"string\",\n          \"description\": \"VM instance type/machine type.\",\n          \"examples\": [\"t3.xlarge\", \"n2-standard-4\", \"Standard_D4s_v3\", \"s-4vcpu-8gb\"]\n        },\n        \"minCount\": {\"type\": \"integer\", \"minimum\": 0, \"description\"\
  : \"Minimum node count.\"},\n        \"maxCount\": {\"type\": \"integer\", \"minimum\": 1, \"description\": \"Maximum node count.\"},\n        \"desiredCount\": {\"type\": \"integer\", \"minimum\": 0, \"description\": \"Desired node count.\"},\n        \"diskSizeGB\": {\"type\": \"integer\", \"minimum\": 20, \"default\": 100},\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\"type\": \"string\"},\n          \"description\": \"Kubernetes node labels.\"\n        },\n        \"taints\": {\n          \"type\": \"array\",\n          \"description\": \"Kubernetes node taints for workload scheduling.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"key\": {\"type\": \"string\"},\n              \"value\": {\"type\": \"string\"},\n              \"effect\": {\"type\": \"string\", \"enum\": [\"NoSchedule\", \"PreferNoSchedule\", \"NoExecute\"]}\n            }\n          }\n        },\n     \
  \   \"spotEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use spot/preemptible instances for cost savings.\",\n          \"default\": false\n        }\n      }\n    },\n    \"ClusterNetworking\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster networking configuration.\",\n      \"properties\": {\n        \"vpcId\": {\"type\": \"string\", \"description\": \"VPC or network ID.\"},\n        \"podCidr\": {\"type\": \"string\", \"description\": \"CIDR block for pod IP addresses.\", \"example\": \"10.244.0.0/16\"},\n        \"serviceCidr\": {\"type\": \"string\", \"description\": \"CIDR block for service cluster IPs.\", \"example\": \"10.96.0.0/12\"},\n        \"cni\": {\n          \"type\": \"string\",\n          \"description\": \"Container Network Interface plugin.\",\n          \"enum\": [\"vpc-cni\", \"calico\", \"cilium\", \"flannel\", \"weave\"],\n          \"default\": \"vpc-cni\"\n        },\n        \"privateCluster\": {\n \
  \         \"type\": \"boolean\",\n          \"description\": \"Whether the API server is accessible only from within the VPC.\",\n          \"default\": false\n        }\n      }\n    },\n    \"ClusterAutoscaling\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster-level autoscaling settings.\",\n      \"properties\": {\n        \"enabled\": {\"type\": \"boolean\", \"default\": true},\n        \"minNodes\": {\"type\": \"integer\", \"minimum\": 1},\n        \"maxNodes\": {\"type\": \"integer\", \"minimum\": 1},\n        \"scaleDownEnabled\": {\"type\": \"boolean\", \"default\": true},\n        \"scaleDownDelayAfterAdd\": {\"type\": \"string\", \"description\": \"Delay after node addition before scale-down.\", \"example\": \"10m\"},\n        \"scaleDownUnneededTime\": {\"type\": \"string\", \"description\": \"Time a node must be unneeded before removal.\", \"example\": \"10m\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/refs/heads/main/json-schema/scalable-infrastructure-kubernetes-cluster-schema.json
tags:
- Cloud Infrastructure
- Compute
- DevOps
- Infrastructure as Code
- Kubernetes
- Networking
- Scalability
- Storage
title: Kubernetes Cluster
---
