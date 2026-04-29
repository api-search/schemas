---
description: UpdateServiceTemplateVersionInput schema from Amazon Proton API
layout: schema
name: UpdateServiceTemplateVersionInput
properties_list:
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
  name: minorVersion
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: supportedComponentSources
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-template-version-input-schema.json
slug: amazon-proton-update-service-template-version-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-template-version-input-schema.json\",\n  \"title\": \"UpdateServiceTemplateVersionInput\",\n  \"description\": \"UpdateServiceTemplateVersionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"compatibleEnvironmentTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompatibleEnvironmentTemplateInputList\"\n        },\n        {\n          \"description\": \"An array of environment template objects that are compatible with this service template version. A service instance based on this service template version can run in environments based on compatible templates.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\
  \n        },\n        {\n          \"description\": \"A description of a service template version to update.\"\n        }\n      ]\n    },\n    \"majorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"To update a major version of a service template, include <code>major Version</code>.\"\n        }\n      ]\n    },\n    \"minorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"To update a minor version of a service template, include <code>minorVersion</code>.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionStatus\"\n        },\n        {\n          \"description\": \"The status of the service template minor version to update.\"\n        }\n      ]\n    },\n    \"supportedComponentSources\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplateSupportedComponentSourceInputList\"\n        },\n        {\n          \"description\": \"<p>An array of supported component sources. Components with supported sources can be attached to service instances based on this service template version.</p> <note> <p>A change to <code>supportedComponentSources</code> doesn't impact existing component attachments to instances based on this template version. A change only affects later associations.</p> </note> <p>For more information about components, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-components.html\\\">Proton components</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"majorVersion\",\n    \"minorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-template-version-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceTemplateVersionInput
---
