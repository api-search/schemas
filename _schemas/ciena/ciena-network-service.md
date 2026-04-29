---
description: Schema representing a provisioned network service on the Blue Planet SDN platform.
layout: schema
name: Ciena Blue Planet Network Service
properties_list:
- description: Unique service identifier (UUID)
  name: id
  type: string
- description: Human-readable service name
  name: name
  type: string
- description: Optional service description
  name: description
  type: string
- description: Service type designation
  name: serviceType
  type: string
- description: Current operational state of the service
  name: state
  type: string
- description: Administrative state
  name: adminState
  type: string
- description: Service bandwidth specification
  name: bandwidth
  type: string
- description: Service protection scheme
  name: protectionType
  type: string
- description: Service termination endpoints (A and Z ends)
  name: endpoints
  type: array
- description: Computed route through the network
  name: route
  type: array
- description: ''
  name: customerInfo
  type: object
- description: Service creation timestamp
  name: createdAt
  type: string
- description: Service provisioning completion timestamp
  name: provisionedAt
  type: string
- description: Last modification timestamp
  name: updatedAt
  type: string
- description: Custom key-value metadata tags
  name: tags
  type: object
provider_name: Ciena
provider_slug: ciena
schema_file: json-schema/ciena-network-service-schema.json
slug: ciena-network-service
source_filename: ciena-network-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.blueplanet.com/schemas/network-service\",\n  \"title\": \"Ciena Blue Planet Network Service\",\n  \"description\": \"Schema representing a provisioned network service on the Blue Planet SDN platform.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"serviceType\", \"state\", \"endpoints\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique service identifier (UUID)\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable service name\",\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional service description\"\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Service type designation\",\n      \"enum\": [\"EPL\", \"EVPL\", \"OTN_ODU\", \"WDM_OCH\"\
  , \"L3VPN\", \"SD_WAN\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state of the service\",\n      \"enum\": [\"ACTIVE\", \"DEGRADED\", \"FAILED\", \"PROVISIONING\", \"DELETING\", \"INACTIVE\"]\n    },\n    \"adminState\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative state\",\n      \"enum\": [\"UNLOCKED\", \"LOCKED\", \"SHUTTING_DOWN\"]\n    },\n    \"bandwidth\": {\n      \"type\": \"string\",\n      \"description\": \"Service bandwidth specification\",\n      \"examples\": [\"1G\", \"10G\", \"100G\", \"400G\"]\n    },\n    \"protectionType\": {\n      \"type\": \"string\",\n      \"description\": \"Service protection scheme\",\n      \"enum\": [\"UNPROTECTED\", \"PROTECTED_1PLUS1\", \"REROUTABLE\", \"RESTORABLE\"]\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"description\": \"Service termination endpoints (A and Z ends)\",\n      \"minItems\": 2,\n      \"maxItems\": 2,\n      \"\
  items\": {\n        \"$ref\": \"#/$defs/ServiceEndpoint\"\n      }\n    },\n    \"route\": {\n      \"type\": \"array\",\n      \"description\": \"Computed route through the network\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RouteHop\"\n      }\n    },\n    \"customerInfo\": {\n      \"$ref\": \"#/$defs/CustomerInfo\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Service creation timestamp\"\n    },\n    \"provisionedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Service provisioning completion timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value metadata tags\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"\
  $defs\": {\n    \"ServiceEndpoint\": {\n      \"type\": \"object\",\n      \"required\": [\"nodeId\", \"portId\", \"direction\"],\n      \"properties\": {\n        \"nodeId\": {\n          \"type\": \"string\",\n          \"description\": \"Network element identifier\"\n        },\n        \"portId\": {\n          \"type\": \"string\",\n          \"description\": \"Port/interface identifier on the node\"\n        },\n        \"direction\": {\n          \"type\": \"string\",\n          \"enum\": [\"A_END\", \"Z_END\"]\n        },\n        \"vlanId\": {\n          \"type\": \"integer\",\n          \"description\": \"VLAN identifier for Ethernet services\",\n          \"minimum\": 1,\n          \"maximum\": 4094\n        },\n        \"innerVlanId\": {\n          \"type\": \"integer\",\n          \"description\": \"Inner VLAN (Q-in-Q) identifier\",\n          \"minimum\": 1,\n          \"maximum\": 4094\n        },\n        \"bandwidth\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Endpoint bandwidth allocation\"\n        }\n      }\n    },\n    \"RouteHop\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"nodeId\": {\n          \"type\": \"string\"\n        },\n        \"linkId\": {\n          \"type\": \"string\"\n        },\n        \"hopOrder\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"CustomerInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"customerId\": {\n          \"type\": \"string\"\n        },\n        \"customerName\": {\n          \"type\": \"string\"\n        },\n        \"serviceOrderId\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/json-schema/ciena-network-service-schema.json
tags:
- MEF
- NETCONF
- Network Automation
- Network Management
- Optical
- RESTCONF
- SDN
- Telecom
- TM Forum
title: Ciena Blue Planet Network Service
---
