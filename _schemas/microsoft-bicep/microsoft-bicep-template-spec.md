---
description: An Azure Template Spec resource that stores reusable Bicep/ARM templates as Azure resources. Template Specs provide versioning, sharing, and access control for infrastructure as code templates compiled from Bicep.
layout: schema
name: Microsoft Bicep Template Spec
properties_list:
- description: The fully qualified Azure resource ID of the Template Spec
  name: id
  type: string
- description: Name of the Template Spec
  name: name
  type: string
- description: The resource type
  name: type
  type: string
- description: The Azure location of the Template Spec. Cannot be changed after creation.
  name: location
  type: string
- description: Resource tags
  name: tags
  type: object
- description: ''
  name: systemData
  type: object
- description: ''
  name: properties
  type: object
provider_name: Microsoft Bicep
provider_slug: microsoft-bicep
schema_file: json-schema/microsoft-bicep-template-spec-schema.json
slug: microsoft-bicep-template-spec
source_filename: microsoft-bicep-template-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://management.azure.com/schemas/microsoft-bicep/template-spec.json\",\n  \"title\": \"Microsoft Bicep Template Spec\",\n  \"description\": \"An Azure Template Spec resource that stores reusable Bicep/ARM templates as Azure resources. Template Specs provide versioning, sharing, and access control for infrastructure as code templates compiled from Bicep.\",\n  \"type\": \"object\",\n  \"required\": [\"location\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The fully qualified Azure resource ID of the Template Spec\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 90,\n      \"pattern\": \"^[-\\\\w\\\\.\\\\_\\\\(\\\\)]+$\",\n      \"description\": \"Name of the Template Spec\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"Microsoft.Resources/templateSpecs\"\
  ,\n      \"description\": \"The resource type\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The Azure location of the Template Spec. Cannot be changed after creation.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource tags\"\n    },\n    \"systemData\": {\n      \"$ref\": \"#/$defs/SystemData\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"maxLength\": 4096,\n          \"description\": \"Template Spec description\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"maxLength\": 64,\n          \"description\": \"Template Spec display name\"\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"The Template Spec metadata, typically a collection\
  \ of key-value pairs\"\n        },\n        \"versions\": {\n          \"type\": \"object\",\n          \"readOnly\": true,\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TemplateSpecVersionInfo\"\n          },\n          \"description\": \"High-level information about the versions within this Template Spec\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"TemplateSpecVersionInfo\": {\n      \"type\": \"object\",\n      \"description\": \"High-level information about a Template Spec version\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Template Spec version description\"\n        },\n        \"timeCreated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true,\n          \"description\": \"The timestamp of when the version was created\"\n        },\n        \"timeModified\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"readOnly\": true,\n          \"description\": \"The timestamp of when the version was last modified\"\n        }\n      }\n    },\n    \"TemplateSpecVersion\": {\n      \"type\": \"object\",\n      \"required\": [\"location\", \"properties\"],\n      \"description\": \"A specific version of a Template Spec containing the compiled template content\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"description\": \"The fully qualified Azure resource ID\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"description\": \"Name of this version\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Microsoft.Resources/templateSpecs/versions\",\n          \"description\": \"The resource type\"\n        },\n        \"location\": {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ Azure location of the Template Spec version\"\n        },\n        \"tags\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Resource tags\"\n        },\n        \"systemData\": {\n          \"$ref\": \"#/$defs/SystemData\"\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"required\": [\"mainTemplate\"],\n          \"properties\": {\n            \"description\": {\n              \"type\": \"string\",\n              \"maxLength\": 4096,\n              \"description\": \"Template Spec version description\"\n            },\n            \"mainTemplate\": {\n              \"type\": \"object\",\n              \"description\": \"The main ARM/Bicep compiled template content\"\n            },\n            \"linkedTemplates\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/LinkedTemplateArtifact\"\n  \
  \            },\n              \"description\": \"Array of linked template artifacts\"\n            },\n            \"metadata\": {\n              \"type\": \"object\",\n              \"description\": \"Version metadata, typically a collection of key-value pairs\"\n            },\n            \"uiFormDefinition\": {\n              \"type\": \"object\",\n              \"description\": \"Azure portal UI form definition for customizing the deployment experience\"\n            }\n          }\n        }\n      }\n    },\n    \"LinkedTemplateArtifact\": {\n      \"type\": \"object\",\n      \"required\": [\"path\", \"template\"],\n      \"description\": \"A linked template artifact within a Template Spec version\",\n      \"properties\": {\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"A filesystem safe relative path of the artifact\"\n        },\n        \"template\": {\n          \"type\": \"object\",\n          \"description\": \"The compiled ARM/Bicep\
  \ template content\"\n        }\n      }\n    },\n    \"SystemData\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata pertaining to creation and last modification of the resource\",\n      \"properties\": {\n        \"createdBy\": {\n          \"type\": \"string\",\n          \"description\": \"The identity that created the resource\"\n        },\n        \"createdByType\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Application\", \"ManagedIdentity\", \"Key\"],\n          \"description\": \"The type of identity that created the resource\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of resource creation (UTC)\"\n        },\n        \"lastModifiedBy\": {\n          \"type\": \"string\",\n          \"description\": \"The identity that last modified the resource\"\n        },\n        \"lastModifiedByType\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"User\", \"Application\", \"ManagedIdentity\", \"Key\"],\n          \"description\": \"The type of identity that last modified the resource\"\n        },\n        \"lastModifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of resource last modification (UTC)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bicep/refs/heads/main/json-schema/microsoft-bicep-template-spec-schema.json
tags:
- ARM Templates
- Azure
- Cloud
- Deployment
- DevOps
- Infrastructure as Code
title: Microsoft Bicep Template Spec
---
