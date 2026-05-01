---
description: ImportVmImageRequest schema from EC2 Image Builder
layout: schema
name: ImportVmImageRequest
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
  name: platform
  type: object
- description: ''
  name: osVersion
  type: object
- description: ''
  name: vmImportTaskId
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-import-vm-image-request-schema.json
slug: ec2-image-builder-import-vm-image-request
source_filename: ec2-image-builder-import-vm-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-import-vm-image-request-schema.json\",\n  \"title\": \"ImportVmImageRequest\",\n  \"description\": \"ImportVmImageRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the base image that is created by the import process.\"\n        }\n      ]\n    },\n    \"semanticVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"<p>The semantic version to attach to the base image that was created during the import process. This version follows the semantic version syntax.</p> <note>\
  \ <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;. You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> </note>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description for the base image that is created by the import process.\"\n        }\n      ]\n    },\n    \"platform\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The operating system platform for the imported VM.\"\n        }\n      ]\n    },\n    \"osVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OsVersion\"\n        },\n        {\n          \"description\": \"The operating system version for the imported VM.\"\n        }\n      ]\n    },\n    \"vmImportTaskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The <code>importTaskId</code> (API) or <code>ImportTaskId</code> (CLI) from the Amazon EC2 VM import process. Image Builder retrieves information from the import process to pull in the AMI that is created from the VM source as the base image for your recipe.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\
  \n        },\n        {\n          \"description\": \"Tags that are attached to the import resources.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier you provide to ensure idempotency of the request. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/Run_Instance_Idempotency.html\\\">Ensuring idempotency</a> in the <i>Amazon EC2 API Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"semanticVersion\",\n    \"platform\",\n    \"vmImportTaskId\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-import-vm-image-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImportVmImageRequest
---
