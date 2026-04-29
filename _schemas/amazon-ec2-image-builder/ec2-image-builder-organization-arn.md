---
description: OrganizationArn schema from EC2 Image Builder
layout: schema
name: OrganizationArn
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-organization-arn-schema.json
slug: ec2-image-builder-organization-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-organization-arn-schema.json\",\n  \"title\": \"OrganizationArn\",\n  \"description\": \"OrganizationArn schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:]*:organizations::[0-9]{12}:organization/o-[a-z0-9]{10,32}$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-organization-arn-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: OrganizationArn
---
