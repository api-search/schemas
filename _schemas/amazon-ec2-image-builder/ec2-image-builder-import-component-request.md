---
description: ImportComponentRequest schema from EC2 Image Builder
layout: schema
name: ImportComponentRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: semanticVersion
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: changeDescription
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: format
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: uri
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-import-component-request-schema.json
slug: ec2-image-builder-import-component-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-import-component-request-schema.json\",\n  \"title\": \"ImportComponentRequest\",\n  \"description\": \"ImportComponentRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"semanticVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"<p>The semantic version of the component. This version follows the semantic version syntax.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;.\
  \ You can assign values for the first three, and can filter on all of them.</p> <p> <b>Filtering:</b> With semantic versioning, you have the flexibility to use wildcards (x) to specify the most recent versions or nodes when selecting the base image or components for your recipe. When you use a wildcard in any node, all nodes to the right of the first wildcard must also be wildcards.</p> </note>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the component. Describes the contents of the component.\"\n        }\n      ]\n    },\n    \"changeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The change description of the component. This description indicates the change that has been made in this version, or what\
  \ makes this version different from other versions of this component.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentType\"\n        },\n        {\n          \"description\": \"The type of the component denotes whether the component is used to build the image, or only to test it.\"\n        }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentFormat\"\n        },\n        {\n          \"description\": \"The format of the resource that you want to import as a component.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The platform of the component.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n\
  \        {\n          \"description\": \"The data of the component. Used to specify the data inline. Either <code>data</code> or <code>uri</code> can be used to specify the data within the component.\"\n        }\n      ]\n    },\n    \"uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uri\"\n        },\n        {\n          \"description\": \"The uri of the component. Must be an Amazon S3 URL and the requester must have permission to access the Amazon S3 bucket. If you use Amazon S3, you can specify component content up to your service quota. Either <code>data</code> or <code>uri</code> can be used to specify the data within the component.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the KMS key that should be used to encrypt this component.\"\n        }\n      ]\n    },\n    \"tags\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the component.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token of the component.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"semanticVersion\",\n    \"type\",\n    \"format\",\n    \"platform\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-import-component-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImportComponentRequest
---
