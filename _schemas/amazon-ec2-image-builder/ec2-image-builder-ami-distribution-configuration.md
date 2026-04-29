---
description: Define and configure the output AMIs of the pipeline.
layout: schema
name: AmiDistributionConfiguration
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: targetAccountIds
  type: object
- description: ''
  name: amiTags
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: launchPermission
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-ami-distribution-configuration-schema.json
slug: ec2-image-builder-ami-distribution-configuration
source_filename: ec2-image-builder-ami-distribution-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ami-distribution-configuration-schema.json\",\n  \"title\": \"AmiDistributionConfiguration\",\n  \"description\": \"Define and configure the output AMIs of the pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiNameString\"\n        },\n        {\n          \"description\": \"The name of the output AMI.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the AMI distribution configuration. Minimum and maximum length are in characters.\"\n        }\n      ]\n    },\n    \"targetAccountIds\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/AccountList\"\n        },\n        {\n          \"description\": \"The ID of an account to which you want to distribute an image.\"\n        }\n      ]\n    },\n    \"amiTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags to apply to AMIs distributed to this Region.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The KMS key identifier used to encrypt the distributed image.\"\n        }\n      ]\n    },\n    \"launchPermission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchPermissionConfiguration\"\n        },\n        {\n          \"description\": \"Launch permissions can be used to configure which Amazon Web Services accounts can use the AMI to\
  \ launch instances.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ami-distribution-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: AmiDistributionConfiguration
---
