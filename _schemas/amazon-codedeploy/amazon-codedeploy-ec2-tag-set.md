---
description: Information about groups of Amazon EC2 instance tags.
layout: schema
name: EC2TagSet
properties_list:
- description: ''
  name: ec2TagSetList
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-ec2-tag-set-schema.json
slug: amazon-codedeploy-ec2-tag-set
source_filename: amazon-codedeploy-ec2-tag-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ec2-tag-set-schema.json\",\n  \"title\": \"EC2TagSet\",\n  \"description\": \"Information about groups of Amazon EC2 instance tags.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ec2TagSetList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagSetList\"\n        },\n        {\n          \"description\": \"A list that contains other lists of Amazon EC2 instance tag groups. For an instance to be included in the deployment group, it must be identified by all of the tag groups in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ec2-tag-set-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: EC2TagSet
---
