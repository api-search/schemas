---
description: UpdateServicePipelineInput schema from Amazon Proton API
layout: schema
name: UpdateServicePipelineInput
properties_list:
- description: ''
  name: deploymentType
  type: object
- description: ''
  name: serviceName
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: templateMajorVersion
  type: object
- description: ''
  name: templateMinorVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-pipeline-input-schema.json
slug: amazon-proton-update-service-pipeline-input
source_filename: amazon-proton-update-service-pipeline-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-pipeline-input-schema.json\",\n  \"title\": \"UpdateServicePipelineInput\",\n  \"description\": \"UpdateServicePipelineInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentUpdateType\"\n        },\n        {\n          \"description\": \"<p>The deployment type.</p> <p>There are four modes for updating a service pipeline. The <code>deploymentType</code> field defines the mode.</p> <dl> <dt/> <dd> <p> <code>NONE</code> </p> <p>In this mode, a deployment <i>doesn't</i> occur. Only the requested metadata parameters are updated.</p> </dd> <dt/> <dd> <p> <code>CURRENT_VERSION</code> </p> <p>In this mode, the service pipeline is deployed and\
  \ updated with the new spec that you provide. Only requested parameters are updated. <i>Don\\u2019t</i> include major or minor version parameters when you use this <code>deployment-type</code>.</p> </dd> <dt/> <dd> <p> <code>MINOR_VERSION</code> </p> <p>In this mode, the service pipeline is deployed and updated with the published, recommended (latest) minor version of the current major version in use, by default. You can specify a different minor version of the current major version in use.</p> </dd> <dt/> <dd> <p> <code>MAJOR_VERSION</code> </p> <p>In this mode, the service pipeline is deployed and updated with the published, recommended (latest) major and minor version of the current template, by default. You can specify a different major version that's higher than the major version in use and a minor version.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n  \
  \      {\n          \"description\": \"The name of the service to that the pipeline is associated with.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The spec for the service pipeline to update.\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The major version of the service template that was used to create the service that the pipeline is associated with.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The minor version of the service template that was used to create the service that the pipeline is associated with.\"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentType\",\n    \"serviceName\",\n    \"spec\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-pipeline-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServicePipelineInput
---
