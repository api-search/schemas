---
description: CreateServiceTemplateVersionInput schema from Amazon Proton API
layout: schema
name: CreateServiceTemplateVersionInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: compatibleEnvironmentTemplates
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: majorVersion
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: supportedComponentSources
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-service-template-version-input-schema.json
slug: amazon-proton-create-service-template-version-input
source_filename: amazon-proton-create-service-template-version-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-template-version-input-schema.json\",\n  \"title\": \"CreateServiceTemplateVersionInput\",\n  \"description\": \"CreateServiceTemplateVersionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"When included, if two identical requests are made with the same client token, Proton returns the service template version that the first request created.\"\n        }\n      ]\n    },\n    \"compatibleEnvironmentTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompatibleEnvironmentTemplateInputList\"\n        },\n        {\n          \"description\":\
  \ \"An array of environment template objects that are compatible with the new service template version. A service instance based on this service template version can run in environments based on compatible templates.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the new version of a service template.\"\n        }\n      ]\n    },\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"<p>To create a new minor version of the service template, include a <code>major Version</code>.</p> <p>To create a new major and minor version of the service template, <i>exclude</i> <code>major Version</code>.</p>\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionSourceInput\"\
  \n        },\n        {\n          \"description\": \"An object that includes the template bundle S3 bucket path and name for the new version of a service template.\"\n        }\n      ]\n    },\n    \"supportedComponentSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplateSupportedComponentSourceInputList\"\n        },\n        {\n          \"description\": \"<p>An array of supported component sources. Components with supported sources can be attached to service instances based on this service template version.</p> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate\
  \ with the Proton service template version. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"compatibleEnvironmentTemplates\",\n    \"source\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-template-version-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateServiceTemplateVersionInput
---
