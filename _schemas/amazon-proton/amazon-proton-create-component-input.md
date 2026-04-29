---
description: CreateComponentInput schema from Amazon Proton API
layout: schema
name: CreateComponentInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: environmentName
  type: object
- description: ''
  name: manifest
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
  name: tags
  type: object
- description: ''
  name: templateFile
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-component-input-schema.json
slug: amazon-proton-create-component-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-component-input-schema.json\",\n  \"title\": \"CreateComponentInput\",\n  \"description\": \"CreateComponentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The client token for the created component.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"An optional customer-provided description of the component.\"\n        }\n      ]\n    },\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the Proton environment that you want to associate this component with. You must specify this when you don't specify <code>serviceInstanceName</code> and <code>serviceName</code>.\"\n        }\n      ]\n    },\n    \"manifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateManifestContents\"\n        },\n        {\n          \"description\": \"A path to a manifest file that lists the Infrastructure as Code (IaC) file, template language, and rendering engine for infrastructure that a custom component provisions.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The customer-provided name of the component.\"\n        }\n      ]\n    },\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the service instance that you want to attach this component to. If you don't specify this, the component isn't attached to any service instance. Specify both <code>serviceInstanceName</code> and <code>serviceName</code> or neither of them.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that <code>serviceInstanceName</code> is associated with. If you don't specify this, the component isn't attached to any service instance. Specify both <code>serviceInstanceName</code> and <code>serviceName</code> or neither of them.\"\n        }\n      ]\n    },\n    \"serviceSpec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The service spec that you want the component\
  \ to use to access service inputs. Set this only when you attach the component to a service instance.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton component. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"templateFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateFileContents\"\n        },\n        {\n          \"description\": \"<p>A path to the Infrastructure as Code (IaC) file describing infrastructure that a custom component provisions.</p> <note> <p>Components support a single IaC file, even if you use Terraform as your template\
  \ language.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"manifest\",\n    \"name\",\n    \"templateFile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-component-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateComponentInput
---
