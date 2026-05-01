---
description: CreateServiceInstanceInput schema from Amazon Proton API
layout: schema
name: CreateServiceInstanceInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: serviceName
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: templateMajorVersion
  type: object
- description: ''
  name: templateMinorVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-service-instance-input-schema.json
slug: amazon-proton-create-service-instance-input
source_filename: amazon-proton-create-service-instance-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-instance-input-schema.json\",\n  \"title\": \"CreateServiceInstanceInput\",\n  \"description\": \"CreateServiceInstanceInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The client token of the service instance to create.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service instance to create.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the service the service instance is added to.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The spec for the service instance you want to create.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton service instance. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\
  \n        },\n        {\n          \"description\": \"To create a new major and minor version of the service template, <i>exclude</i> <code>major Version</code>.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"To create a new minor version of the service template, include a <code>major Version</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"serviceName\",\n    \"spec\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-instance-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateServiceInstanceInput
---
