---
description: Response for creating an EC2 environment.
layout: schema
name: CreateEnvironmentEC2Response
properties_list:
- description: The ID of the environment that was created.
  name: environmentId
  type: string
provider_name: Amazon Cloud9
provider_slug: amazon-cloud9
schema_file: json-schema/cloud9-create-environment-ec2-response-schema.json
slug: cloud9-create-environment-ec2-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-create-environment-ec2-response-schema.json\",\n  \"title\": \"CreateEnvironmentEC2Response\",\n  \"description\": \"Response for creating an EC2 environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the environment that was created.\",\n      \"example\": \"abc12345678901234567890\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-create-environment-ec2-response-schema.json
tags:
- AWS
- Cloud9
- IDE
- Development
- Browser-Based
title: CreateEnvironmentEC2Response
---
