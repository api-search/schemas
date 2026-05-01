---
description: Represents a package installed on an Image Builder image.
layout: schema
name: ImagePackage
properties_list:
- description: ''
  name: packageName
  type: object
- description: ''
  name: packageVersion
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-package-schema.json
slug: ec2-image-builder-image-package
source_filename: ec2-image-builder-image-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-package-schema.json\",\n  \"title\": \"ImagePackage\",\n  \"description\": \"Represents a package installed on an Image Builder image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the package as reported to the operating system package manager.\"\n        }\n      ]\n    },\n    \"packageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The version of the package as reported to the operating system package manager.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-package-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImagePackage
---
