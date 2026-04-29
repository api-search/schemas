---
description: The base resource model for Azure Resource Manager resources. All Azure resources inherit from this schema, which defines the standard properties shared by all Azure resource types including ID, name, type, location, tags, and system metadata.
layout: schema
name: Azure Resource
properties_list:
- description: Fully qualified resource ID for the resource. The format is /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: The type of the resource, in the format {resourceProviderNamespace}/{resourceType}.
  name: type
  type: string
- description: The geo-location where the resource lives. Must be one of the supported Azure regions.
  name: location
  type: string
- description: Resource tags. Key-value pairs used to organize and categorize Azure resources for billing, management, and automation purposes.
  name: tags
  type: object
- description: The fully qualified resource ID of the resource that manages this resource. Used when a resource is managed by another Azure resource.
  name: managedBy
  type: string
- description: The kind of the resource. Metadata used by the portal/tooling/etc. to render different UX experiences for resources of the same type.
  name: kind
  type: string
- description: Resource Etag for optimistic concurrency control.
  name: etag
  type: string
- description: ''
  name: identity
  type: object
- description: ''
  name: sku
  type: object
- description: ''
  name: plan
  type: object
- description: The availability zones for the resource.
  name: zones
  type: array
- description: ''
  name: systemData
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/microsoft-azure-resource-schema.json
slug: microsoft-azure-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-azure/resource\",\n  \"title\": \"Azure Resource\",\n  \"description\": \"The base resource model for Azure Resource Manager resources. All Azure resources inherit from this schema, which defines the standard properties shared by all Azure resource types including ID, name, type, location, tags, and system metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID for the resource. The format is /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/myResourceGroup/providers/Microsoft.Compute/virtualMachines/myVM\"\n      ]\n    },\n    \"name\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The name of the resource.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"myVM\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource, in the format {resourceProviderNamespace}/{resourceType}.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"Microsoft.Compute/virtualMachines\"\n      ]\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives. Must be one of the supported Azure regions.\",\n      \"examples\": [\n        \"eastus\",\n        \"westus2\",\n        \"westeurope\",\n        \"southeastasia\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags. Key-value pairs used to organize and categorize Azure resources for billing, management, and automation purposes.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\
  \n      },\n      \"examples\": [\n        {\n          \"environment\": \"production\",\n          \"department\": \"engineering\",\n          \"cost-center\": \"12345\"\n        }\n      ]\n    },\n    \"managedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified resource ID of the resource that manages this resource. Used when a resource is managed by another Azure resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of the resource. Metadata used by the portal/tooling/etc. to render different UX experiences for resources of the same type.\",\n      \"pattern\": \"^[-\\\\w\\\\._,\\\\(\\\\)]+$\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Resource Etag for optimistic concurrency control.\",\n      \"readOnly\": true\n    },\n    \"identity\": {\n      \"$ref\": \"#/$defs/ManagedServiceIdentity\"\n    },\n    \"sku\": {\n      \"$ref\": \"#/$defs/Sku\"\n    },\n    \"plan\"\
  : {\n      \"$ref\": \"#/$defs/Plan\"\n    },\n    \"zones\": {\n      \"type\": \"array\",\n      \"description\": \"The availability zones for the resource.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"1\", \"2\", \"3\"]\n      ]\n    },\n    \"systemData\": {\n      \"$ref\": \"#/$defs/SystemData\"\n    }\n  },\n  \"required\": [\n    \"location\"\n  ],\n  \"$defs\": {\n    \"ManagedServiceIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"Managed service identity (system assigned and/or user assigned identities).\",\n      \"properties\": {\n        \"principalId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The service principal ID of the system assigned identity.\",\n          \"readOnly\": true\n        },\n        \"tenantId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The tenant ID of the system assigned\
  \ identity.\",\n          \"readOnly\": true\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of managed service identity.\",\n          \"enum\": [\n            \"None\",\n            \"SystemAssigned\",\n            \"UserAssigned\",\n            \"SystemAssigned, UserAssigned\"\n          ]\n        },\n        \"userAssignedIdentities\": {\n          \"type\": \"object\",\n          \"description\": \"The set of user assigned identities associated with the resource. Dictionary keys are ARM resource IDs.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/UserAssignedIdentity\"\n          }\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"UserAssignedIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"User assigned identity properties.\",\n      \"properties\": {\n        \"principalId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n\
  \          \"description\": \"The principal ID of the assigned identity.\",\n          \"readOnly\": true\n        },\n        \"clientId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The client ID of the assigned identity.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"Sku\": {\n      \"type\": \"object\",\n      \"description\": \"The resource model definition representing SKU.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the SKU. E.g., P3. It is typically a letter+number code.\"\n        },\n        \"tier\": {\n          \"type\": \"string\",\n          \"description\": \"This field is required to be implemented by the Resource Provider if the service has more than one tier.\",\n          \"enum\": [\n            \"Free\",\n            \"Basic\",\n            \"Standard\",\n            \"Premium\"\n          ]\n        },\n     \
  \   \"size\": {\n          \"type\": \"string\",\n          \"description\": \"The SKU size. When the name field is the combination of tier and some other value, this would be the standalone code.\"\n        },\n        \"family\": {\n          \"type\": \"string\",\n          \"description\": \"If the service has different generations of hardware, for the same SKU, then that can be captured here.\"\n        },\n        \"capacity\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"description\": \"If the SKU supports scale out/in then the capacity integer should be included.\"\n        }\n      },\n      \"required\": [\n        \"name\"\n      ]\n    },\n    \"Plan\": {\n      \"type\": \"object\",\n      \"description\": \"Plan for the resource.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"A user defined name of the 3rd Party Artifact that is being procured.\"\n        },\n        \"\
  publisher\": {\n          \"type\": \"string\",\n          \"description\": \"The publisher of the 3rd Party Artifact that is being bought.\"\n        },\n        \"product\": {\n          \"type\": \"string\",\n          \"description\": \"The 3rd Party artifact that is being procured.\"\n        },\n        \"promotionCode\": {\n          \"type\": \"string\",\n          \"description\": \"A publisher provided promotion code.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the desired product/artifact.\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"publisher\",\n        \"product\"\n      ]\n    },\n    \"SystemData\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata pertaining to creation and last modification of the resource.\",\n      \"properties\": {\n        \"createdBy\": {\n          \"type\": \"string\",\n          \"description\": \"The identity that created the\
  \ resource.\"\n        },\n        \"createdByType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of identity that created the resource.\",\n          \"enum\": [\n            \"User\",\n            \"Application\",\n            \"ManagedIdentity\",\n            \"Key\"\n          ]\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of resource creation (UTC).\"\n        },\n        \"lastModifiedBy\": {\n          \"type\": \"string\",\n          \"description\": \"The identity that last modified the resource.\"\n        },\n        \"lastModifiedByType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of identity that last modified the resource.\",\n          \"enum\": [\n            \"User\",\n            \"Application\",\n            \"ManagedIdentity\",\n            \"Key\"\n          ]\n        },\n        \"lastModifiedAt\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of resource last modification (UTC).\"\n        }\n      },\n      \"readOnly\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/microsoft-azure-resource-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Azure Resource
---
