---
description: UserDataOverride schema from EC2 Image Builder
layout: schema
name: UserDataOverride
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-user-data-override-schema.json
slug: ec2-image-builder-user-data-override
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-user-data-override-schema.json\",\n  \"title\": \"UserDataOverride\",\n  \"description\": \"UserDataOverride schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$\",\n  \"minLength\": 1,\n  \"maxLength\": 21847\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-user-data-override-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: UserDataOverride
---
