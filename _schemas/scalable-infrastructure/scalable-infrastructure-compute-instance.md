---
description: A normalized schema describing a cloud compute instance (VM/Droplet/Node) across providers such as AWS EC2, Google Compute Engine, Azure VMs, and DigitalOcean Droplets.
layout: schema
name: Compute Instance
properties_list:
- description: Provider-assigned unique instance identifier.
  name: id
  type: string
- description: Human-readable name for the instance.
  name: name
  type: string
- description: Cloud provider hosting this instance.
  name: provider
  type: string
- description: Instance type/size (e.g., t3.medium, n2-standard-4, Standard_D2s_v3, s-2vcpu-4gb).
  name: type
  type: string
- description: Current lifecycle state of the instance.
  name: status
  type: string
- description: Cloud region where the instance is deployed (e.g., us-east-1, us-central1, eastus, nyc3).
  name: region
  type: string
- description: Specific availability zone within the region.
  name: availabilityZone
  type: string
- description: ID of the OS image (AMI, Compute Image, Marketplace Image).
  name: imageId
  type: string
- description: Operating system details.
  name: os
  type: object
- description: ''
  name: cpu
  type: object
- description: ''
  name: memory
  type: object
- description: Attached block storage volumes.
  name: storage
  type: array
- description: ''
  name: networking
  type: object
- description: GPU details for GPU-enabled instances.
  name: gpu
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: terminatedAt
  type: string
provider_name: Scalable Infrastructure
provider_slug: scalable-infrastructure
schema_file: json-schema/scalable-infrastructure-compute-instance-schema.json
slug: scalable-infrastructure-compute-instance
source_filename: scalable-infrastructure-compute-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/main/json-schema/scalable-infrastructure-compute-instance-schema.json\",\n  \"title\": \"Compute Instance\",\n  \"description\": \"A normalized schema describing a cloud compute instance (VM/Droplet/Node) across providers such as AWS EC2, Google Compute Engine, Azure VMs, and DigitalOcean Droplets.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"provider\", \"type\", \"status\", \"region\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Provider-assigned unique instance identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the instance.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider hosting this instance.\",\n      \"enum\": [\"aws\", \"gcp\", \"azure\"\
  , \"digitalocean\", \"linode\", \"hetzner\", \"vultr\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Instance type/size (e.g., t3.medium, n2-standard-4, Standard_D2s_v3, s-2vcpu-4gb).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the instance.\",\n      \"enum\": [\"pending\", \"running\", \"stopping\", \"stopped\", \"terminated\", \"rebooting\", \"error\"]\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where the instance is deployed (e.g., us-east-1, us-central1, eastus, nyc3).\"\n    },\n    \"availabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"Specific availability zone within the region.\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the OS image (AMI, Compute Image, Marketplace Image).\"\n    },\n    \"os\": {\n      \"type\": \"object\",\n      \"description\": \"Operating\
  \ system details.\",\n      \"properties\": {\n        \"family\": {\n          \"type\": \"string\",\n          \"enum\": [\"Linux\", \"Windows\", \"BSD\"],\n          \"default\": \"Linux\"\n        },\n        \"distribution\": {\n          \"type\": \"string\",\n          \"examples\": [\"Ubuntu 24.04 LTS\", \"Amazon Linux 2023\", \"Debian 12\", \"RHEL 9\", \"Windows Server 2022\"]\n        }\n      }\n    },\n    \"cpu\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"vCPUs\": {\"type\": \"integer\", \"minimum\": 1},\n        \"architecture\": {\"type\": \"string\", \"enum\": [\"x86_64\", \"arm64\", \"x86_32\"]}\n      }\n    },\n    \"memory\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sizeGiB\": {\"type\": \"number\", \"minimum\": 0},\n        \"type\": {\"type\": \"string\", \"enum\": [\"DDR4\", \"DDR5\", \"HBM2\", \"standard\"]}\n      }\n    },\n    \"storage\": {\n      \"type\": \"array\",\n      \"description\": \"Attached block\
  \ storage volumes.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"volumeId\": {\"type\": \"string\"},\n          \"type\": {\"type\": \"string\", \"enum\": [\"ssd\", \"hdd\", \"nvme\", \"network-ssd\", \"network-hdd\"]},\n          \"sizeGiB\": {\"type\": \"integer\", \"minimum\": 1},\n          \"iops\": {\"type\": \"integer\"},\n          \"isRoot\": {\"type\": \"boolean\"}\n        }\n      }\n    },\n    \"networking\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"vpcId\": {\"type\": \"string\"},\n        \"subnetId\": {\"type\": \"string\"},\n        \"privateIp\": {\"type\": \"string\", \"format\": \"ipv4\"},\n        \"publicIp\": {\"type\": \"string\", \"format\": \"ipv4\"},\n        \"ipv6\": {\"type\": \"string\", \"format\": \"ipv6\"},\n        \"securityGroups\": {\n          \"type\": \"array\",\n          \"items\": {\"type\": \"string\"}\n        },\n        \"bandwidthGbps\": {\"type\": \"number\"}\n \
  \     }\n    },\n    \"gpu\": {\n      \"type\": \"object\",\n      \"description\": \"GPU details for GPU-enabled instances.\",\n      \"properties\": {\n        \"count\": {\"type\": \"integer\", \"minimum\": 1},\n        \"model\": {\"type\": \"string\", \"examples\": [\"NVIDIA A100\", \"NVIDIA H100\", \"NVIDIA T4\", \"AMD MI300X\"]},\n        \"memoryGiB\": {\"type\": \"number\"}\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\"type\": \"string\"}\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"terminatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/refs/heads/main/json-schema/scalable-infrastructure-compute-instance-schema.json
tags:
- Cloud Infrastructure
- Compute
- DevOps
- Infrastructure as Code
- Kubernetes
- Networking
- Scalability
- Storage
title: Compute Instance
---
