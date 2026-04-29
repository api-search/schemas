---
description: A container encapsulates the runtime environment for an application.
layout: schema
name: Container
properties_list:
- description: ''
  name: region
  type: object
- description: ''
  name: imageUris
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-container-schema.json
slug: ec2-image-builder-container
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-schema.json\",\n  \"title\": \"Container\",\n  \"description\": \"A container encapsulates the runtime environment for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Containers and container images are Region-specific. This is the Region context for the container.\"\n        }\n      ]\n    },\n    \"imageUris\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"A list of URIs for containers created in the context Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Container
---
