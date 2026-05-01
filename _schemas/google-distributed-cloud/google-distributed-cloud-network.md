---
description: Schema for a Distributed Cloud edge network resource used to define network configurations in edge deployments.
layout: schema
name: Google Distributed Cloud Edge Network
properties_list:
- description: The resource name of the network
  name: name
  type: string
- description: Timestamp when the network was created
  name: createTime
  type: string
- description: Timestamp when the network was last updated
  name: updateTime
  type: string
- description: Labels applied to the network
  name: labels
  type: object
- description: User-provided description of the network
  name: description
  type: string
- description: Maximum transmission unit in bytes
  name: mtu
  type: integer
- description: Subnets associated with this network
  name: subnets
  type: array
- description: Routers associated with this network
  name: routers
  type: array
provider_name: Google Distributed Cloud
provider_slug: google-distributed-cloud
schema_file: json-schema/google-distributed-cloud-network-schema.json
slug: google-distributed-cloud-network
source_filename: google-distributed-cloud-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/distributedcloud/network.json\",\n  \"title\": \"Google Distributed Cloud Edge Network\",\n  \"description\": \"Schema for a Distributed Cloud edge network resource used to define network configurations in edge deployments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the network\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the network was created\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the network was last updated\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels applied\
  \ to the network\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-provided description of the network\"\n    },\n    \"mtu\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum transmission unit in bytes\",\n      \"minimum\": 1280,\n      \"maximum\": 9000\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Subnet\"\n      },\n      \"description\": \"Subnets associated with this network\"\n    },\n    \"routers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Router\"\n      },\n      \"description\": \"Routers associated with this network\"\n    }\n  },\n  \"$defs\": {\n    \"Subnet\": {\n      \"type\": \"object\",\n      \"description\": \"A subnet within an edge network\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the subnet\"\n        },\n        \"network\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The parent network resource name\"\n        },\n        \"ipv4Cidr\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"pattern\": \"^([0-9]{1,3}\\\\.){3}[0-9]{1,3}/[0-9]{1,2}$\"\n          },\n          \"description\": \"IPv4 CIDR ranges for the subnet\"\n        },\n        \"ipv6Cidr\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"IPv6 CIDR ranges for the subnet\"\n        },\n        \"vlanId\": {\n          \"type\": \"integer\",\n          \"description\": \"VLAN ID for the subnet\",\n          \"minimum\": 1,\n          \"maximum\": 4094\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"User-provided description\"\n        }\n      }\n    },\n    \"Router\": {\n      \"type\": \"object\",\n      \"description\": \"\
  A router within an edge network\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the router\"\n        },\n        \"network\": {\n          \"type\": \"string\",\n          \"description\": \"The parent network resource name\"\n        },\n        \"bgpPeers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/BgpPeer\"\n          },\n          \"description\": \"BGP peer configurations\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"BgpPeer\": {\n      \"type\": \"object\",\n      \"description\": \"A BGP peer configuration for a router\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the BGP peer\"\n        },\n        \"peerIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"IP address of the BGP peer\"\n  \
  \      },\n        \"peerAsn\": {\n          \"type\": \"integer\",\n          \"description\": \"ASN of the BGP peer\",\n          \"minimum\": 1\n        },\n        \"localAsn\": {\n          \"type\": \"integer\",\n          \"description\": \"Local ASN for this peer session\",\n          \"minimum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-distributed-cloud/refs/heads/main/json-schema/google-distributed-cloud-network-schema.json
tags:
- Distributed Infrastructure
- Edge Computing
- Hardware
- Hybrid Cloud
- Kubernetes
- On-Premises
title: Google Distributed Cloud Edge Network
---
