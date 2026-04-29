---
description: Detail data for a provisioned resource.
layout: schema
name: ProvisionedResource
properties_list:
- description: ''
  name: identifier
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: provisioningEngine
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-provisioned-resource-schema.json
slug: amazon-proton-provisioned-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-provisioned-resource-schema.json\",\n  \"title\": \"ProvisionedResource\",\n  \"description\": \"Detail data for a provisioned resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedResourceIdentifier\"\n        },\n        {\n          \"description\": \"The provisioned resource identifier.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedResourceName\"\n        },\n        {\n          \"description\": \"The provisioned resource name.\"\n        }\n      ]\n    },\n    \"provisioningEngine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedResourceEngine\"\
  \n        },\n        {\n          \"description\": \"<p>The resource provisioning engine. At this time, <code>CLOUDFORMATION</code> can be used for Amazon Web Services-managed provisioning, and <code>TERRAFORM</code> can be used for self-managed provisioning.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-works-prov-methods.html#ag-works-prov-methods-self\\\">Self-managed provisioning</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-provisioned-resource-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ProvisionedResource
---
