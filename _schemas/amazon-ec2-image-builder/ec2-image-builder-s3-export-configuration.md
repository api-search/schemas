---
description: Properties that configure export from your build instance to a compatible file format for your VM.
layout: schema
name: S3ExportConfiguration
properties_list:
- description: ''
  name: roleName
  type: object
- description: ''
  name: diskImageFormat
  type: object
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3Prefix
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-s3-export-configuration-schema.json
slug: ec2-image-builder-s3-export-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-s3-export-configuration-schema.json\",\n  \"title\": \"S3ExportConfiguration\",\n  \"description\": \"Properties that configure export from your build instance to a compatible file format for your VM.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the role that grants VM Import/Export permission to export images to your S3 bucket.\"\n        }\n      ]\n    },\n    \"diskImageFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskImageFormat\"\n        },\n        {\n          \"description\": \"<p>Export the updated image to one of the following supported disk image\
  \ formats:</p> <ul> <li> <p> <b>Virtual Hard Disk (VHD)</b> \\u2013 Compatible with Citrix Xen and Microsoft Hyper-V virtualization products.</p> </li> <li> <p> <b>Stream-optimized ESX Virtual Machine Disk (VMDK)</b> \\u2013 Compatible with VMware ESX and VMware vSphere versions 4, 5, and 6.</p> </li> <li> <p> <b>Raw</b> \\u2013 Raw format.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"s3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The S3 bucket in which to store the output disk images for your VM.\"\n        }\n      ]\n    },\n    \"s3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon S3 path for the bucket where the output disk images for your VM are stored.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"roleName\",\n    \"diskImageFormat\"\
  ,\n    \"s3Bucket\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-s3-export-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: S3ExportConfiguration
---
