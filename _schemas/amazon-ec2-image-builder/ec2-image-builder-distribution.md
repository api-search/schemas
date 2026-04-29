---
description: Defines the settings for a specific Region.
layout: schema
name: Distribution
properties_list:
- description: ''
  name: region
  type: object
- description: ''
  name: amiDistributionConfiguration
  type: object
- description: ''
  name: containerDistributionConfiguration
  type: object
- description: ''
  name: licenseConfigurationArns
  type: object
- description: ''
  name: launchTemplateConfigurations
  type: object
- description: ''
  name: s3ExportConfiguration
  type: object
- description: ''
  name: fastLaunchConfigurations
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-distribution-schema.json
slug: ec2-image-builder-distribution
source_filename: ec2-image-builder-distribution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-distribution-schema.json\",\n  \"title\": \"Distribution\",\n  \"description\": \"Defines the settings for a specific Region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The target Region.\"\n        }\n      ]\n    },\n    \"amiDistributionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiDistributionConfiguration\"\n        },\n        {\n          \"description\": \"The specific AMI settings; for example, launch permissions or AMI tags.\"\n        }\n      ]\n    },\n    \"containerDistributionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ContainerDistributionConfiguration\"\n        },\n        {\n          \"description\": \"Container distribution settings for encryption, licensing, and sharing in a specific Region.\"\n        }\n      ]\n    },\n    \"licenseConfigurationArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LicenseConfigurationArnList\"\n        },\n        {\n          \"description\": \"The License Manager Configuration to associate with the AMI in the specified Region.\"\n        }\n      ]\n    },\n    \"launchTemplateConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateConfigurationList\"\n        },\n        {\n          \"description\": \"A group of launchTemplateConfiguration settings that apply to image distribution for specified accounts.\"\n        }\n      ]\n    },\n    \"s3ExportConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ExportConfiguration\"\
  \n        },\n        {\n          \"description\": \"Configure export settings to deliver disk images created from your image build, using a file format that is compatible with your VMs in that Region.\"\n        }\n      ]\n    },\n    \"fastLaunchConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FastLaunchConfigurationList\"\n        },\n        {\n          \"description\": \"The Windows faster-launching configurations to use for AMI distribution.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"region\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-distribution-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Distribution
---
