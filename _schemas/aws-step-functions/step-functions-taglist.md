---
description: ''
layout: schema
name: TagList
properties_list: []
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-taglist-schema.json
slug: step-functions-taglist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"key\": {},\n      \"value\": {}\n    },\n    \"description\": \"<p>Tags are key-value pairs that can be associated with Step Functions state machines and activities.</p> <p>An array of key-value pairs. For more information, see <a href=\\\"https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-alloc-tags.html\\\">Using Cost Allocation Tags</a> in the <i>Amazon Web Services Billing and Cost Management User Guide</i>, and <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_iam-tags.html\\\">Controlling Access Using IAM Tags</a>.</p> <p>Tags may only contain Unicode letters, digits, white space, or these symbols: <code>_ . : / = + - @</code>.</p>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-taglist-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: TagList
---
