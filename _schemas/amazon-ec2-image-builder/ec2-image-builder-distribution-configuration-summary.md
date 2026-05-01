---
description: A high-level overview of a distribution configuration.
layout: schema
name: DistributionConfigurationSummary
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
  name: dateCreated
  type: object
- description: ''
  name: dateUpdated
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: regions
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-distribution-configuration-summary-schema.json
slug: ec2-image-builder-distribution-configuration-summary
source_filename: ec2-image-builder-distribution-configuration-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-distribution-configuration-summary-schema.json\",\n  \"title\": \"DistributionConfigurationSummary\",\n  \"description\": \"A high-level overview of a distribution configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the distribution configuration.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the distribution configuration.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the distribution configuration.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which the distribution configuration was created.\"\n        }\n      ]\n    },\n    \"dateUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which the distribution configuration was updated.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags associated with the distribution configuration.\"\n        }\n      ]\n    },\n    \"regions\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/RegionList\"\n        },\n        {\n          \"description\": \"A list of Regions where the container image is distributed to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-distribution-configuration-summary-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: DistributionConfigurationSummary
---
