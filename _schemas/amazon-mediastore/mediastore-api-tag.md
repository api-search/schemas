---
description: A collection of tags associated with a container. Each tag consists of a key:value pair, which can be anything you define. Typically, the tag key represents a category (such as "environment") and the tag value represents a specific value within that category (such as "test," "development," or "production"). You can add up to 50 tags to each container. For more information about tagging, including naming and usage conventions, see <a href="https://docs.aws.amazon.com/mediastore/latest/ug/tagging.html">Tagging Resources in MediaStore</a>.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-tag-schema.json
slug: mediastore-api-tag
source_filename: mediastore-api-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A collection of tags associated with a container. Each tag consists of a key:value pair, which can be anything you define. Typically, the tag key represents a category (such as \\\"environment\\\") and the tag value represents a specific value within that category (such as \\\"test,\\\" \\\"development,\\\" or \\\"production\\\"). You can add up to 50 tags to each container. For more information about tagging, including naming and usage conventions, see <a href=\\\"https://docs.aws.amazon.com/mediastore/latest/ug/tagging.html\\\">Tagging Resources in MediaStore</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n\
  \        {\n          \"description\": \"Part of the key:value pair that defines a tag. You can use a tag key to describe a category of information, such as \\\"customer.\\\" Tag keys are case-sensitive.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"Part of the key:value pair that defines a tag. You can use a tag value to describe a specific value within a category, such as \\\"companyA\\\" or \\\"companyB.\\\" Tag values are case-sensitive.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Tag
---
