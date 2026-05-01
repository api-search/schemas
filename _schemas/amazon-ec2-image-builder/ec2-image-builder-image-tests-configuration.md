---
description: Configure image tests for your pipeline build. Tests run after building the image, to verify that the AMI or container image is valid before distributing it.
layout: schema
name: ImageTestsConfiguration
properties_list:
- description: ''
  name: imageTestsEnabled
  type: object
- description: ''
  name: timeoutMinutes
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-tests-configuration-schema.json
slug: ec2-image-builder-image-tests-configuration
source_filename: ec2-image-builder-image-tests-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-tests-configuration-schema.json\",\n  \"title\": \"ImageTestsConfiguration\",\n  \"description\": \"Configure image tests for your pipeline build. Tests run after building the image, to verify that the AMI or container image is valid before distributing it.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageTestsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Determines if tests should run after building the image. Image Builder defaults to enable tests to run following the image build, before image distribution.\"\n        }\n      ]\n    },\n    \"timeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageTestsTimeoutMinutes\"\
  \n        },\n        {\n          \"description\": \"<p>The maximum time in minutes that tests are permitted to run.</p> <note> <p>The timeoutMinutes attribute is not currently active. This value is ignored.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-tests-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageTestsConfiguration
---
