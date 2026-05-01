---
description: AssociationArn schema from Amazon CodeGuru Reviewer
layout: schema
name: AssociationArn
properties_list: []
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-association-arn-schema.json
slug: amazon-codeguru-reviewer-association-arn
source_filename: amazon-codeguru-reviewer-association-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-association-arn-schema.json\",\n  \"title\": \"AssociationArn\",\n  \"description\": \"AssociationArn schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:\\\\s]*:codeguru-reviewer:[^:\\\\s]+:[\\\\d]{12}:association:[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-association-arn-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: AssociationArn
---
