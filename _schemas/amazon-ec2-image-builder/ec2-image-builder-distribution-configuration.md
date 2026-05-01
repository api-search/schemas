---
description: A distribution configuration.
layout: schema
name: DistributionConfiguration
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: distributions
  type: object
- description: ''
  name: timeoutMinutes
  type: object
- description: ''
  name: dateCreated
  type: object
- description: ''
  name: dateUpdated
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-distribution-configuration-schema.json
slug: ec2-image-builder-distribution-configuration
source_filename: ec2-image-builder-distribution-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-distribution-configuration-schema.json\",\n  \"title\": \"DistributionConfiguration\",\n  \"description\": \"A distribution configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the distribution configuration.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the distribution configuration.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\
  \n        },\n        {\n          \"description\": \"The description of the distribution configuration.\"\n        }\n      ]\n    },\n    \"distributions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DistributionList\"\n        },\n        {\n          \"description\": \"The distribution objects that apply Region-specific settings for the deployment of the image to targeted Regions.\"\n        }\n      ]\n    },\n    \"timeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DistributionTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The maximum duration in minutes for this distribution configuration.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which this distribution configuration was created.\"\n        }\n      ]\n    },\n    \"dateUpdated\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which this distribution configuration was last updated.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the distribution configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timeoutMinutes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-distribution-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: DistributionConfiguration
---
