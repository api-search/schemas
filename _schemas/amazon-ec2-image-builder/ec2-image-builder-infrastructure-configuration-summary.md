---
description: The infrastructure used when building Amazon EC2 AMIs.
layout: schema
name: InfrastructureConfigurationSummary
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
  name: resourceTags
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: instanceTypes
  type: object
- description: ''
  name: instanceProfileName
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-infrastructure-configuration-summary-schema.json
slug: ec2-image-builder-infrastructure-configuration-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-infrastructure-configuration-summary-schema.json\",\n  \"title\": \"InfrastructureConfigurationSummary\",\n  \"description\": \"The infrastructure used when building Amazon EC2 AMIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which the infrastructure configuration was created.\"\n        }\n      ]\n    },\n    \"dateUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which the infrastructure configuration was last updated.\"\n        }\n      ]\n    },\n    \"resourceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagMap\"\n        },\n        {\n          \"description\": \"The tags attached to the image created by Image Builder.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"instanceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeList\"\n        },\n        {\n          \"description\": \"The instance types of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"instanceProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceProfileNameType\"\n        },\n        {\n          \"description\": \"The instance profile of the infrastructure configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-infrastructure-configuration-summary-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: InfrastructureConfigurationSummary
---
