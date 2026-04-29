---
description: Returns information about the resource being evaluated.
layout: schema
name: ResourceDetails
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ResourceConfiguration
  type: object
- description: ''
  name: ResourceConfigurationSchemaType
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-details-schema.json
slug: config-resource-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-details-schema.json\",\n  \"title\": \"ResourceDetails\",\n  \"description\": \"Returns information about the resource being evaluated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseResourceId\"\n        },\n        {\n          \"description\": \"A unique resource ID for an evaluation.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The type of resource being evaluated.\"\n        }\n      ]\n    },\n    \"ResourceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceConfiguration\"\
  \n        },\n        {\n          \"description\": \"The resource definition to be evaluated as per the resource configuration schema type.\"\n        }\n      ]\n    },\n    \"ResourceConfigurationSchemaType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceConfigurationSchemaType\"\n        },\n        {\n          \"description\": \"<p>The schema type of the resource configuration.</p> <note> <p>You can find the <a href=\\\"https://docs.aws.amazon.com/cloudformation-cli/latest/userguide/resource-type-schema.html\\\">Resource type schema</a>, or <code>CFN_RESOURCE_SCHEMA</code>, in \\\"<i>Amazon Web Services public extensions</i>\\\" within the CloudFormation registry or with the following CLI commmand: <code>aws cloudformation describe-type --type-name \\\"AWS::S3::Bucket\\\" --type RESOURCE</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html#registry-view\\\">Managing\
  \ extensions through the CloudFormation registry</a> and <a href=\\\"https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html\\\">Amazon Web Services resource and property types reference</a> in the CloudFormation User Guide.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\",\n    \"ResourceType\",\n    \"ResourceConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-details-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceDetails
---
