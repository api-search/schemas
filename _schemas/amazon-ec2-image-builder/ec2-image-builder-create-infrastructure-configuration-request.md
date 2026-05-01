---
description: CreateInfrastructureConfigurationRequest schema from EC2 Image Builder
layout: schema
name: CreateInfrastructureConfigurationRequest
properties_list:
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
  name: resourceTags
  type: object
- description: ''
  name: instanceMetadataOptions
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-create-infrastructure-configuration-request-schema.json
slug: ec2-image-builder-create-infrastructure-configuration-request
source_filename: ec2-image-builder-create-infrastructure-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-infrastructure-configuration-request-schema.json\",\n  \"title\": \"CreateInfrastructureConfigurationRequest\",\n  \"description\": \"CreateInfrastructureConfigurationRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"instanceTypes\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeList\"\n        },\n        {\n          \"description\": \"The instance types of the infrastructure configuration. You can specify one or more instance types to use for this build. The service will pick one of these instance types based on availability.\"\n        }\n      ]\n    },\n    \"instanceProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceProfileNameType\"\n        },\n        {\n          \"description\": \"The instance profile to associate with the instance used to customize your Amazon EC2 AMI.\"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The security group IDs to associate with the instance used to customize your Amazon EC2 AMI.\"\n        }\n      ]\n    },\n    \"subnetId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The subnet ID in which to place the instance used to customize your Amazon EC2 AMI.\"\n        }\n      ]\n    },\n    \"logging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Logging\"\n        },\n        {\n          \"description\": \"The logging configuration of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"keyPair\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The key pair of the infrastructure configuration. You can use this to log on to and debug the instance used to create your image.\"\n        }\n      ]\n    },\n    \"terminateInstanceOnFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\"\
  : \"The terminate instance on failure setting of the infrastructure configuration. Set to false if you want Image Builder to retain the instance used to configure your AMI if the build or test phase of your workflow fails.\"\n        }\n      ]\n    },\n    \"snsTopicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopicArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) for the SNS topic to which we send image build event notifications.</p> <note> <p>EC2 Image Builder is unable to send notifications to SNS topics that are encrypted using keys from other accounts. The key that is used to encrypt the SNS topic must reside in the account that the Image Builder service runs under.</p> </note>\"\n        }\n      ]\n    },\n    \"resourceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagMap\"\n        },\n        {\n          \"description\": \"The tags attached to the\
  \ resource created by Image Builder.\"\n        }\n      ]\n    },\n    \"instanceMetadataOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataOptions\"\n        },\n        {\n          \"description\": \"The instance metadata options that you can set for the HTTP requests that pipeline builds use to launch EC2 build and test instances.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the infrastructure configuration.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token used to make this request idempotent.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"instanceProfileName\",\n    \"clientToken\"\n \
  \ ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-infrastructure-configuration-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CreateInfrastructureConfigurationRequest
---
