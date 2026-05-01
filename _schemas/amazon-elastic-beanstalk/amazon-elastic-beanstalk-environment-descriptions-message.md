---
description: EnvironmentDescriptionsMessage schema from Amazon Elastic Beanstalk AWS Elastic Beanstalk API
layout: schema
name: EnvironmentDescriptionsMessage
properties_list:
- description: ''
  name: Environments
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Elastic Beanstalk
provider_slug: amazon-elastic-beanstalk
schema_file: json-schema/amazon-elastic-beanstalk-environment-descriptions-message-schema.json
slug: amazon-elastic-beanstalk-environment-descriptions-message
source_filename: amazon-elastic-beanstalk-environment-descriptions-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-environment-descriptions-message-schema.json\",\n  \"title\": \"EnvironmentDescriptionsMessage\",\n  \"description\": \"EnvironmentDescriptionsMessage schema from Amazon Elastic Beanstalk AWS Elastic Beanstalk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Environments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Environment\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-environment-descriptions-message-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Deployment
- Elastic Beanstalk
- PaaS
- Platform As A Service
- Web Applications
title: EnvironmentDescriptionsMessage
---
