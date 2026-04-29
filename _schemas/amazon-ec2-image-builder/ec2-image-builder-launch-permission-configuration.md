---
description: Describes the configuration for a launch permission. The launch permission modification request is sent to the <a href="https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifyImageAttribute.html">Amazon EC2 ModifyImageAttribute</a> API on behalf of the user for each Region they have selected to distribute the AMI. To make an AMI public, set the launch permission authorized accounts to <code>all</code>. See the examples for making an AMI public at <a href="https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifyImageAttribute.html">Amazon EC2 ModifyImageAttribute</a>.
layout: schema
name: LaunchPermissionConfiguration
properties_list:
- description: ''
  name: userIds
  type: object
- description: ''
  name: userGroups
  type: object
- description: ''
  name: organizationArns
  type: object
- description: ''
  name: organizationalUnitArns
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-launch-permission-configuration-schema.json
slug: ec2-image-builder-launch-permission-configuration
source_filename: ec2-image-builder-launch-permission-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-launch-permission-configuration-schema.json\",\n  \"title\": \"LaunchPermissionConfiguration\",\n  \"description\": \"Describes the configuration for a launch permission. The launch permission modification request is sent to the <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifyImageAttribute.html\\\">Amazon EC2 ModifyImageAttribute</a> API on behalf of the user for each Region they have selected to distribute the AMI. To make an AMI public, set the launch permission authorized accounts to <code>all</code>. See the examples for making an AMI public at <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifyImageAttribute.html\\\">Amazon EC2 ModifyImageAttribute</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userIds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"userGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"organizationArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationArnList\"\n        },\n        {\n          \"description\": \"The ARN for an Amazon Web Services Organization that you want to share your AMI with. For more information, see <a href=\\\"https://docs.aws.amazon.com/organizations/latest/userguide/orgs_introduction.html\\\">What is Organizations?</a>.\"\n        }\n      ]\n    },\n    \"organizationalUnitArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationalUnitArnList\"\
  \n        },\n        {\n          \"description\": \"The ARN for an Organizations organizational unit (OU) that you want to share your AMI with. For more information about key concepts for Organizations, see <a href=\\\"https://docs.aws.amazon.com/organizations/latest/userguide/orgs_getting-started_concepts.html\\\">Organizations terminology and concepts</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-launch-permission-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: LaunchPermissionConfiguration
---
