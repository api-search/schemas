---
description: Details of the infrastructure configuration.
layout: schema
name: InfrastructureConfiguration
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
  name: instanceTypes
  type: object
- description: ''
  name: instanceProfileName
  type: object
- description: ''
  name: securityGroupIds
  type: object
- description: ''
  name: subnetId
  type: object
- description: ''
  name: logging
  type: object
- description: ''
  name: keyPair
  type: object
- description: ''
  name: terminateInstanceOnFailure
  type: object
- description: ''
  name: snsTopicArn
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
  name: instanceMetadataOptions
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-infrastructure-configuration-schema.json
slug: ec2-image-builder-infrastructure-configuration
source_filename: ec2-image-builder-infrastructure-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-infrastructure-configuration-schema.json\",\n  \"title\": \"InfrastructureConfiguration\",\n  \"description\": \"Details of the infrastructure configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\
  \n        },\n        {\n          \"description\": \"The description of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"instanceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeList\"\n        },\n        {\n          \"description\": \"The instance types of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"instanceProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceProfileNameType\"\n        },\n        {\n          \"description\": \"The instance profile of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The security group IDs of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"subnetId\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The subnet ID of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"logging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Logging\"\n        },\n        {\n          \"description\": \"The logging configuration of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"keyPair\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon EC2 key pair of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"terminateInstanceOnFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"The terminate instance on failure configuration of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"snsTopicArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) for the SNS topic to which we send image build event notifications.</p> <note> <p>EC2 Image Builder is unable to send notifications to SNS topics that are encrypted using keys from other accounts. The key that is used to encrypt the SNS topic must reside in the account that the Image Builder service runs under.</p> </note>\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which the infrastructure configuration was created.\"\n        }\n      ]\n    },\n    \"dateUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which the infrastructure configuration\
  \ was last updated.\"\n        }\n      ]\n    },\n    \"resourceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagMap\"\n        },\n        {\n          \"description\": \"The tags attached to the resource created by Image Builder.\"\n        }\n      ]\n    },\n    \"instanceMetadataOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataOptions\"\n        },\n        {\n          \"description\": \"The instance metadata option settings for the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the infrastructure configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-infrastructure-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: InfrastructureConfiguration
---
