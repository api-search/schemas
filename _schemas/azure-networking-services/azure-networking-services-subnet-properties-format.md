---
description: Properties of the subnet.
layout: schema
name: SubnetPropertiesFormat
properties_list:
- description: The address prefix for the subnet.
  name: addressPrefix
  type: string
- description: List of address prefixes for the subnet.
  name: addressPrefixes
  type: array
- description: An array of references to the delegations on the subnet.
  name: delegations
  type: array
- description: Array of IP configuration profiles which reference this subnet.
  name: ipConfigurationProfiles
  type: array
- description: An array of references to the network interface IP configurations using subnet.
  name: ipConfigurations
  type: array
- description: Reference to another subresource.
  name: natGateway
  type: object
- description: The reference of the NetworkSecurityGroup resource.
  name: networkSecurityGroup
  type: object
- description: Enable or Disable apply network policies on private end point in the subnet.
  name: privateEndpointNetworkPolicies
  type: string
- description: An array of references to private endpoints.
  name: privateEndpoints
  type: array
- description: Enable or Disable apply network policies on private link service in the subnet.
  name: privateLinkServiceNetworkPolicies
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: A read-only string identifying the intention of use for this subnet based on delegations and other user-defined properties.
  name: purpose
  type: string
- description: An array of references to the external resources using subnet.
  name: resourceNavigationLinks
  type: array
- description: The reference of the RouteTable resource.
  name: routeTable
  type: object
- description: An array of references to services injecting into this subnet.
  name: serviceAssociationLinks
  type: array
- description: An array of service endpoint policies.
  name: serviceEndpointPolicies
  type: array
- description: An array of service endpoints.
  name: serviceEndpoints
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-subnet-properties-format-schema.json
slug: azure-networking-services-subnet-properties-format
source_filename: azure-networking-services-subnet-properties-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-subnet-properties-format-schema.json\",\n  \"title\": \"SubnetPropertiesFormat\",\n  \"description\": \"Properties of the subnet.\",\n  \"properties\": {\n    \"addressPrefix\": {\n      \"description\": \"The address prefix for the subnet.\",\n      \"type\": \"string\"\n    },\n    \"addressPrefixes\": {\n      \"description\": \"List of address prefixes for the subnet.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"delegations\": {\n      \"description\": \"An array of references to the delegations on the subnet.\",\n      \"items\": {\n        \"allOf\": [\n          {\n            \"description\": \"Reference to another subresource.\",\n            \"properties\": {\n              \"id\": {\n            \
  \    \"description\": \"Resource ID.\",\n                \"type\": \"string\"\n              }\n            },\n            \"x-ms-azure-resource\": true\n          }\n        ],\n        \"description\": \"Details the service to which the subnet is delegated.\",\n        \"properties\": {\n          \"etag\": {\n            \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"The name of the resource that is unique within a subnet. This name can be used to access the resource.\",\n            \"type\": \"string\"\n          },\n          \"properties\": {\n            \"description\": \"Properties of a service delegation.\",\n            \"properties\": {\n              \"actions\": {\n                \"description\": \"Describes the actions permitted to the service upon delegation.\",\n                \"items\": {\n                  \"type\"\
  : \"string\"\n                },\n                \"type\": \"array\"\n              },\n              \"provisioningState\": {\n                \"description\": \"The current provisioning state.\",\n                \"enum\": [\n                  \"Succeeded\",\n                  \"Updating\",\n                  \"Deleting\",\n                  \"Failed\"\n                ],\n                \"readOnly\": true,\n                \"type\": \"string\",\n                \"x-ms-enum\": {\n                  \"modelAsString\": true,\n                  \"name\": \"ProvisioningState\"\n                }\n              },\n              \"serviceName\": {\n                \"description\": \"The name of the service to whom the subnet should be delegated (e.g. Microsoft.Sql/servers).\",\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      },\n      \"type\": \"array\"\n    },\n    \"ipConfigurationProfiles\": {\n      \"description\": \"Array of IP configuration\
  \ profiles which reference this subnet.\",\n      \"items\": {\n        \"$ref\": \"./networkProfile.json#/definitions/IPConfigurationProfile\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"ipConfigurations\": {\n      \"description\": \"An array of references to the network interface IP configurations using subnet.\",\n      \"items\": {\n        \"$ref\": \"./networkInterface.json#/definitions/IPConfiguration\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"natGateway\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"networkSecurityGroup\": {\n      \"$ref\": \"./networkSecurityGroup.json#/definitions/NetworkSecurityGroup\",\n      \"description\": \"The reference of the NetworkSecurityGroup resource.\"\n    },\n\
  \    \"privateEndpointNetworkPolicies\": {\n      \"description\": \"Enable or Disable apply network policies on private end point in the subnet.\",\n      \"type\": \"string\"\n    },\n    \"privateEndpoints\": {\n      \"description\": \"An array of references to private endpoints.\",\n      \"items\": {\n        \"$ref\": \"./privateEndpoint.json#/definitions/PrivateEndpoint\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"privateLinkServiceNetworkPolicies\": {\n      \"description\": \"Enable or Disable apply network policies on private link service in the subnet.\",\n      \"type\": \"string\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\
  \n      }\n    },\n    \"purpose\": {\n      \"description\": \"A read-only string identifying the intention of use for this subnet based on delegations and other user-defined properties.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"resourceNavigationLinks\": {\n      \"description\": \"An array of references to the external resources using subnet.\",\n      \"items\": {\n        \"allOf\": [\n          {\n            \"description\": \"Reference to another subresource.\",\n            \"properties\": {\n              \"id\": {\n                \"description\": \"Resource ID.\",\n                \"type\": \"string\"\n              }\n            },\n            \"x-ms-azure-resource\": true\n          }\n        ],\n        \"description\": \"ResourceNavigationLink resource.\",\n        \"properties\": {\n          \"etag\": {\n            \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n            \"readOnly\"\
  : true,\n            \"type\": \"string\"\n          },\n          \"id\": {\n            \"description\": \"Resource navigation link identifier.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"Name of the resource that is unique within a resource group. This name can be used to access the resource.\",\n            \"type\": \"string\"\n          },\n          \"properties\": {\n            \"description\": \"Properties of ResourceNavigationLink.\",\n            \"properties\": {\n              \"link\": {\n                \"description\": \"Link to the external resource.\",\n                \"type\": \"string\"\n              },\n              \"linkedResourceType\": {\n                \"description\": \"Resource type of the linked resource.\",\n                \"type\": \"string\"\n              },\n              \"provisioningState\": {\n                \"description\": \"The current provisioning\
  \ state.\",\n                \"enum\": [\n                  \"Succeeded\",\n                  \"Updating\",\n                  \"Deleting\",\n                  \"Failed\"\n                ],\n                \"readOnly\": true,\n                \"type\": \"string\",\n                \"x-ms-enum\": {\n                  \"modelAsString\": true,\n                  \"name\": \"ProvisioningState\"\n                }\n              }\n            }\n          },\n          \"type\": {\n            \"description\": \"Resource type.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"type\": \"array\"\n    },\n    \"routeTable\": {\n      \"$ref\": \"./routeTable.json#/definitions/RouteTable\",\n      \"description\": \"The reference of the RouteTable resource.\"\n    },\n    \"serviceAssociationLinks\": {\n      \"description\": \"An array of references to services injecting into this subnet.\",\n      \"items\": {\n        \"allOf\"\
  : [\n          {\n            \"description\": \"Reference to another subresource.\",\n            \"properties\": {\n              \"id\": {\n                \"description\": \"Resource ID.\",\n                \"type\": \"string\"\n              }\n            },\n            \"x-ms-azure-resource\": true\n          }\n        ],\n        \"description\": \"ServiceAssociationLink resource.\",\n        \"properties\": {\n          \"etag\": {\n            \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"Name of the resource that is unique within a resource group. This name can be used to access the resource.\",\n            \"type\": \"string\"\n          },\n          \"properties\": {\n            \"description\": \"Properties of ServiceAssociationLink.\",\n            \"properties\": {\n              \"\
  allowDelete\": {\n                \"description\": \"If true, the resource can be deleted.\",\n                \"type\": \"boolean\"\n              },\n              \"link\": {\n                \"description\": \"Link to the external resource.\",\n                \"type\": \"string\"\n              },\n              \"linkedResourceType\": {\n                \"description\": \"Resource type of the linked resource.\",\n                \"type\": \"string\"\n              },\n              \"locations\": {\n                \"description\": \"A list of locations.\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"type\": \"array\"\n              },\n              \"provisioningState\": {\n                \"description\": \"The current provisioning state.\",\n                \"enum\": [\n                  \"Succeeded\",\n                  \"Updating\",\n                  \"Deleting\",\n                  \"Failed\"\n             \
  \   ],\n                \"readOnly\": true,\n                \"type\": \"string\",\n                \"x-ms-enum\": {\n                  \"modelAsString\": true,\n                  \"name\": \"ProvisioningState\"\n                }\n              }\n            }\n          },\n          \"type\": {\n            \"description\": \"Resource type.\",\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"type\": \"array\"\n    },\n    \"serviceEndpointPolicies\": {\n      \"description\": \"An array of service endpoint policies.\",\n      \"items\": {\n        \"$ref\": \"./serviceEndpointPolicy.json#/definitions/ServiceEndpointPolicy\"\n      },\n      \"type\": \"array\"\n    },\n    \"serviceEndpoints\": {\n      \"description\": \"An array of service endpoints.\",\n      \"items\": {\n        \"description\": \"The service endpoint properties.\",\n        \"properties\": {\n          \"locations\": {\n            \"description\": \"A list of locations.\",\n     \
  \       \"items\": {\n              \"type\": \"string\"\n            },\n            \"type\": \"array\"\n          },\n          \"provisioningState\": {\n            \"description\": \"The current provisioning state.\",\n            \"enum\": [\n              \"Succeeded\",\n              \"Updating\",\n              \"Deleting\",\n              \"Failed\"\n            ],\n            \"readOnly\": true,\n            \"type\": \"string\",\n            \"x-ms-enum\": {\n              \"modelAsString\": true,\n              \"name\": \"ProvisioningState\"\n            }\n          },\n          \"service\": {\n            \"description\": \"The type of the endpoint service.\",\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-subnet-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: SubnetPropertiesFormat
---
