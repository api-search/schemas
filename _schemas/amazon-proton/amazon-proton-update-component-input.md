---
description: UpdateComponentInput schema from Amazon Proton API
layout: schema
name: UpdateComponentInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: deploymentType
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
- description: ''
  name: serviceSpec
  type: object
- description: ''
  name: templateFile
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-component-input-schema.json
slug: amazon-proton-update-component-input
source_filename: amazon-proton-update-component-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-component-input-schema.json\",\n  \"title\": \"UpdateComponentInput\",\n  \"description\": \"UpdateComponentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The client token for the updated component.\"\n        }\n      ]\n    },\n    \"deploymentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentDeploymentUpdateType\"\n        },\n        {\n          \"description\": \"<p>The deployment type. It defines the mode for updating a component, as follows:</p> <dl> <dt/> <dd> <p> <code>NONE</code> </p> <p>In this mode, a deployment <i>doesn't</i>\
  \ occur. Only the requested metadata parameters are updated. You can only specify <code>description</code> in this mode.</p> </dd> <dt/> <dd> <p> <code>CURRENT_VERSION</code> </p> <p>In this mode, the component is deployed and updated with the new <code>serviceSpec</code>, <code>templateSource</code>, and/or <code>type</code> that you provide. Only requested parameters are updated.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"An optional customer-provided description of the component.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the component to update.\"\n        }\n      ]\n    },\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/ResourceNameOrEmpty\"\n        },\n        {\n          \"description\": \"The name of the service instance that you want to attach this component to. Don't specify to keep the component's current service instance attachment. Specify an empty string to detach the component from the service instance it's attached to. Specify non-empty values for both <code>serviceInstanceName</code> and <code>serviceName</code> or for neither of them.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceNameOrEmpty\"\n        },\n        {\n          \"description\": \"The name of the service that <code>serviceInstanceName</code> is associated with. Don't specify to keep the component's current service instance attachment. Specify an empty string to detach the component from the service instance it's attached to. Specify non-empty values for both <code>serviceInstanceName</code> and <code>serviceName</code>\
  \ or for neither of them.\"\n        }\n      ]\n    },\n    \"serviceSpec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The service spec that you want the component to use to access service inputs. Set this only when the component is attached to a service instance.\"\n        }\n      ]\n    },\n    \"templateFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateFileContents\"\n        },\n        {\n          \"description\": \"<p>A path to the Infrastructure as Code (IaC) file describing infrastructure that a custom component provisions.</p> <note> <p>Components support a single IaC file, even if you use Terraform as your template language.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentType\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-component-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateComponentInput
---
