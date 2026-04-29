---
description: PutResourceConfigRequest schema
layout: schema
name: PutResourceConfigRequest
properties_list:
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: SchemaVersionId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ResourceName
  type: object
- description: ''
  name: Configuration
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-resource-config-request-schema.json
slug: config-put-resource-config-request
source_filename: config-put-resource-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-resource-config-request-schema.json\",\n  \"title\": \"PutResourceConfigRequest\",\n  \"description\": \"PutResourceConfigRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypeString\"\n        },\n        {\n          \"description\": \"<p>The type of the resource. The custom resource type must be registered with CloudFormation. </p> <note> <p>You cannot use the organization names \\u201camzn\\u201d, \\u201camazon\\u201d, \\u201calexa\\u201d, \\u201ccustom\\u201d with custom resource types. It is the first part of the ResourceType up to the first ::.</p> </note>\"\n        }\n      ]\n    },\n    \"SchemaVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/SchemaVersionId\"\n        },\n        {\n          \"description\": \"Version of the schema registered for the ResourceType in CloudFormation.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"Unique identifier of the resource.\"\n        }\n      ]\n    },\n    \"ResourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"Name of the resource.\"\n        }\n      ]\n    },\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Configuration\"\n        },\n        {\n          \"description\": \"<p>The configuration object of the resource in valid JSON format. It must match the schema registered with CloudFormation.</p> <note> <p>The configuration JSON must not exceed 64 KB.</p>\
  \ </note>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>Tags associated with the resource.</p> <note> <p>This field is not to be confused with the Amazon Web Services-wide tag feature for Amazon Web Services resources. Tags for <code>PutResourceConfig</code> are tags that you supply for the configuration items of your custom resources.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceType\",\n    \"SchemaVersionId\",\n    \"ResourceId\",\n    \"Configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-resource-config-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutResourceConfigRequest
---
