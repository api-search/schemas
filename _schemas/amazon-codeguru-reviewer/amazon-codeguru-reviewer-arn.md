---
description: Arn schema from Amazon CodeGuru Reviewer
layout: schema
name: Arn
properties_list: []
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-arn-schema.json
slug: amazon-codeguru-reviewer-arn
source_filename: amazon-codeguru-reviewer-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-arn-schema.json\",\n  \"title\": \"Arn\",\n  \"description\": \"Arn schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:\\\\s]*:codeguru-reviewer:[^:\\\\s]+:[\\\\d]{12}:[a-z-]+:[\\\\w-]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-arn-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: Arn
---
