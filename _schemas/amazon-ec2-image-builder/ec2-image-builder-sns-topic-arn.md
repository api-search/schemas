---
description: SnsTopicArn schema from EC2 Image Builder
layout: schema
name: SnsTopicArn
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-sns-topic-arn-schema.json
slug: ec2-image-builder-sns-topic-arn
source_filename: ec2-image-builder-sns-topic-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-sns-topic-arn-schema.json\",\n  \"title\": \"SnsTopicArn\",\n  \"description\": \"SnsTopicArn schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:]*:sns:[^:]+:[0-9]{12}:[a-zA-Z0-9-_]{1,256}$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-sns-topic-arn-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: SnsTopicArn
---
