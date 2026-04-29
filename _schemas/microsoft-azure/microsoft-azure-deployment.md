---
description: An Azure Resource Manager deployment represents the process of deploying one or more resources to an Azure subscription, resource group, or management group. Deployments use ARM templates (JSON or Bicep) to define the resources to deploy, their configurations, and dependencies.
layout: schema
name: Azure Resource Manager Deployment
properties_list:
- description: The ID of the deployment.
  name: id
  type: string
- description: The name of the deployment.
  name: name
  type: string
- description: The type of the deployment.
  name: type
  type: string
- description: The location to store the deployment data.
  name: location
  type: string
- description: Deployment properties.
  name: properties
  type: object
- description: Deployment tags.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/microsoft-azure-deployment-schema.json
slug: microsoft-azure-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-azure/deployment\",\n  \"title\": \"Azure Resource Manager Deployment\",\n  \"description\": \"An Azure Resource Manager deployment represents the process of deploying one or more resources to an Azure subscription, resource group, or management group. Deployments use ARM templates (JSON or Bicep) to define the resources to deploy, their configurations, and dependencies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the deployment.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the deployment.\",\n      \"readOnly\": true,\n      \"minLength\": 1,\n      \"maxLength\": 64,\n      \"pattern\": \"^[-\\\\w\\\\._\\\\(\\\\)]+$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ type of the deployment.\",\n      \"readOnly\": true,\n      \"const\": \"Microsoft.Resources/deployments\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location to store the deployment data.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Deployment properties.\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"Denotes the state of provisioning.\",\n          \"readOnly\": true,\n          \"enum\": [\n            \"NotSpecified\",\n            \"Accepted\",\n            \"Running\",\n            \"Ready\",\n            \"Creating\",\n            \"Created\",\n            \"Deleting\",\n            \"Deleted\",\n            \"Canceled\",\n            \"Failed\",\n            \"Succeeded\",\n            \"Updating\"\n          ]\n        },\n        \"correlationId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The correlation ID of the deployment.\",\n          \"readOnly\": true\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of the template deployment.\",\n          \"readOnly\": true\n        },\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"The duration of the template deployment.\",\n          \"readOnly\": true\n        },\n        \"outputs\": {\n          \"type\": \"object\",\n          \"description\": \"Key/value pairs that represent deployment output.\",\n          \"readOnly\": true\n        },\n        \"template\": {\n          \"type\": \"object\",\n          \"description\": \"The template content. Use this element when you want to pass the template syntax directly in the request rather than link to an existing template.\"\n        },\n        \"templateLink\": {\n          \"type\": \"object\",\n          \"description\": \"The\
  \ URI of the template. Use this element to link to an existing template rather than including the template in the request.\",\n          \"properties\": {\n            \"uri\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The URI of the template to deploy.\"\n            },\n            \"contentVersion\": {\n              \"type\": \"string\",\n              \"description\": \"If included, must match the ContentVersion in the template.\",\n              \"pattern\": \"^(\\\\d+\\\\.)(\\\\d+\\\\.)(\\\\d+\\\\.)(\\\\d+)$\"\n            },\n            \"queryString\": {\n              \"type\": \"string\",\n              \"description\": \"The query string to use with the templateLink URI.\"\n            }\n          },\n          \"required\": [\n            \"uri\"\n          ]\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"description\": \"Name and value pairs that define the deployment\
  \ parameters. The parameters are passed directly to the template.\"\n        },\n        \"parametersLink\": {\n          \"type\": \"object\",\n          \"description\": \"The URI of parameters file. Use this element to link to an existing parameters file.\",\n          \"properties\": {\n            \"uri\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The URI of the parameters file.\"\n            },\n            \"contentVersion\": {\n              \"type\": \"string\",\n              \"description\": \"If included, must match the ContentVersion in the parameters file.\"\n            }\n          },\n          \"required\": [\n            \"uri\"\n          ]\n        },\n        \"mode\": {\n          \"type\": \"string\",\n          \"description\": \"The mode that is used to deploy resources. Incremental mode handles deployments as incremental updates. Complete mode deletes resources that exist in the resource group\
  \ but are not specified in the template.\",\n          \"enum\": [\n            \"Incremental\",\n            \"Complete\"\n          ]\n        },\n        \"debugSetting\": {\n          \"type\": \"object\",\n          \"description\": \"The debug setting of the deployment.\",\n          \"properties\": {\n            \"detailLevel\": {\n              \"type\": \"string\",\n              \"description\": \"Specifies the type of information to log for debugging. The permitted values are none, requestContent, responseContent, or both requestContent and responseContent separated by a comma.\"\n            }\n          }\n        },\n        \"onErrorDeployment\": {\n          \"type\": \"object\",\n          \"description\": \"The deployment on error behavior.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The deployment on error behavior type.\",\n              \"enum\": [\n                \"LastSuccessful\"\
  ,\n                \"SpecificDeployment\"\n              ]\n            },\n            \"deploymentName\": {\n              \"type\": \"string\",\n              \"description\": \"The deployment to be used on error case.\"\n            }\n          }\n        }\n      },\n      \"required\": [\n        \"mode\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Deployment tags.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/microsoft-azure-deployment-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Azure Resource Manager Deployment
---
