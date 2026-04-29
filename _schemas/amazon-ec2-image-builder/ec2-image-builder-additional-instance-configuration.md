---
description: <p>In addition to your infrastructure configuration, these settings provide an extra layer of control over your build instances. You can also specify commands to run on launch for all of your build instances.</p> <p>Image Builder does not automatically install the Systems Manager agent on Windows instances. If your base image includes the Systems Manager agent, then the AMI that you create will also include the agent. For Linux instances, if the base image does not already include the Systems Manager agent, Image Builder installs it. For Linux instances where Image Builder installs the Systems Manager agent, you can choose whether to keep it for the AMI that you create.</p>
layout: schema
name: AdditionalInstanceConfiguration
properties_list:
- description: ''
  name: systemsManagerAgent
  type: object
- description: ''
  name: userDataOverride
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-additional-instance-configuration-schema.json
slug: ec2-image-builder-additional-instance-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-additional-instance-configuration-schema.json\",\n  \"title\": \"AdditionalInstanceConfiguration\",\n  \"description\": \"<p>In addition to your infrastructure configuration, these settings provide an extra layer of control over your build instances. You can also specify commands to run on launch for all of your build instances.</p> <p>Image Builder does not automatically install the Systems Manager agent on Windows instances. If your base image includes the Systems Manager agent, then the AMI that you create will also include the agent. For Linux instances, if the base image does not already include the Systems Manager agent, Image Builder installs it. For Linux instances where Image Builder installs the Systems Manager agent, you can choose whether to keep it for the AMI that\
  \ you create.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"systemsManagerAgent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SystemsManagerAgent\"\n        },\n        {\n          \"description\": \"Contains settings for the Systems Manager agent on your build instance.\"\n        }\n      ]\n    },\n    \"userDataOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserDataOverride\"\n        },\n        {\n          \"description\": \"<p>Use this property to provide commands or a command script to run when you launch your build instance.</p> <p>The userDataOverride property replaces any commands that Image Builder might have added to ensure that Systems Manager is installed on your Linux build instance. If you override the user data, make sure that you add commands to install Systems Manager, if it is not pre-installed on your base image.</p> <note> <p>The user data is always base 64 encoded. For example,\
  \ the following commands are encoded as <code>IyEvYmluL2Jhc2gKbWtkaXIgLXAgL3Zhci9iYi8KdG91Y2ggL3Zhci$</code>:</p> <p> <i>#!/bin/bash</i> </p> <p>mkdir -p /var/bb/</p> <p>touch /var</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-additional-instance-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: AdditionalInstanceConfiguration
---
