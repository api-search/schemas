---
description: Describes the launch template and the version of the launch template that Amazon EC2 Auto Scaling uses to launch Amazon EC2 instances. For more information about launch templates, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/LaunchTemplates.html">Launch templates</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.
layout: schema
name: LaunchTemplateSpecification
properties_list:
- description: ''
  name: LaunchTemplateId
  type: object
- description: ''
  name: LaunchTemplateName
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-launch-template-specification-schema.json
slug: ec2-auto-scaling-launch-template-specification
source_filename: ec2-auto-scaling-launch-template-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-template-specification-schema.json\",\n  \"title\": \"LaunchTemplateSpecification\",\n  \"description\": \"Describes the launch template and the version of the launch template that Amazon EC2 Auto Scaling uses to launch Amazon EC2 instances. For more information about launch templates, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/LaunchTemplates.html\\\">Launch templates</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The ID of the launch template. To get the template ID, use the Amazon EC2 <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeLaunchTemplates.html\\\
  \">DescribeLaunchTemplates</a> API operation. New launch templates can be created using the Amazon EC2 <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateLaunchTemplate.html\\\">CreateLaunchTemplate</a> API. </p> <p>Conditional: You must specify either a <code>LaunchTemplateId</code> or a <code>LaunchTemplateName</code>.</p>\"\n        }\n      ]\n    },\n    \"LaunchTemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateName\"\n        },\n        {\n          \"description\": \"<p>The name of the launch template. To get the template name, use the Amazon EC2 <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeLaunchTemplates.html\\\">DescribeLaunchTemplates</a> API operation. New launch templates can be created using the Amazon EC2 <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateLaunchTemplate.html\\\">CreateLaunchTemplate</a> API. </p> <p>Conditional:\
  \ You must specify either a <code>LaunchTemplateId</code> or a <code>LaunchTemplateName</code>.</p>\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The version number, <code>$Latest</code>, or <code>$Default</code>. To get the version number, use the Amazon EC2 <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeLaunchTemplateVersions.html\\\">DescribeLaunchTemplateVersions</a> API operation. New launch template versions can be created using the Amazon EC2 <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateLaunchTemplateVersion.html\\\">CreateLaunchTemplateVersion</a> API. If the value is <code>$Latest</code>, Amazon EC2 Auto Scaling selects the latest version of the launch template when launching instances. If the value is <code>$Default</code>, Amazon EC2 Auto Scaling selects the default\
  \ version of the launch template when launching instances. The default value is <code>$Default</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-template-specification-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: LaunchTemplateSpecification
---
