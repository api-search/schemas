---
description: ListServiceInstanceProvisionedResourcesInput schema from Amazon Proton API
layout: schema
name: ListServiceInstanceProvisionedResourcesInput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-instance-provisioned-resources-input-schema.json
slug: amazon-proton-list-service-instance-provisioned-resources-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instance-provisioned-resources-input-schema.json\",\n  \"title\": \"ListServiceInstanceProvisionedResourcesInput\",\n  \"description\": \"ListServiceInstanceProvisionedResourcesInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next provisioned resource in the array of provisioned resources, after the list of provisioned resources that was previously requested.\"\n        }\n      ]\n    },\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n   \
  \       \"description\": \"The name of the service instance whose provisioned resources you want.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that <code>serviceInstanceName</code> is associated to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceInstanceName\",\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instance-provisioned-resources-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServiceInstanceProvisionedResourcesInput
---
