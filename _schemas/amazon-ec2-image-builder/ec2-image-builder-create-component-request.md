---
description: CreateComponentRequest schema from EC2 Image Builder
layout: schema
name: CreateComponentRequest
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
  name: platform
  type: object
- description: ''
  name: supportedOsVersions
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
schema_file: json-schema/ec2-image-builder-create-component-request-schema.json
slug: ec2-image-builder-create-component-request
source_filename: ec2-image-builder-create-component-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-component-request-schema.json\",\n  \"title\": \"CreateComponentRequest\",\n  \"description\": \"CreateComponentRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"semanticVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"<p>The semantic version of the component. This version follows the semantic version syntax.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;.\
  \ You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> </note>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Describes the contents of the component.\"\n        }\n      ]\n    },\n    \"changeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"\
  description\": \"The change description of the component. Describes what change has been made in this version, or what makes this version different from other versions of this component.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The operating system platform of the component.\"\n        }\n      ]\n    },\n    \"supportedOsVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OsVersionList\"\n        },\n        {\n          \"description\": \"The operating system (OS) version supported by the component. If the OS information is available, a prefix match is performed against the base image OS version during image recipe creation.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InlineComponentData\"\n        },\n        {\n          \"\
  description\": \"Component <code>data</code> contains inline YAML document content for the component. Alternatively, you can specify the <code>uri</code> of a YAML document file stored in Amazon S3. However, you cannot specify both properties.\"\n        }\n      ]\n    },\n    \"uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uri\"\n        },\n        {\n          \"description\": \"<p>The <code>uri</code> of a YAML component document file. This must be an S3 URL (<code>s3://bucket/key</code>), and the requester must have permission to access the S3 bucket it points to. If you use Amazon S3, you can specify component content up to your service quota.</p> <p>Alternatively, you can specify the YAML document inline, using the component <code>data</code> property. You cannot specify both properties.</p>\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n      \
  \  },\n        {\n          \"description\": \"The ID of the KMS key that is used to encrypt this component.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags that apply to the component.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token of the component.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"semanticVersion\",\n    \"platform\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-component-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CreateComponentRequest
---
