---
description: ApplicationDescriptionsMessage schema from Amazon Elastic Beanstalk AWS Elastic Beanstalk API
layout: schema
name: ApplicationDescriptionsMessage
properties_list:
- description: ''
  name: Applications
  type: array
provider_name: Amazon Elastic Beanstalk
provider_slug: amazon-elastic-beanstalk
schema_file: json-schema/amazon-elastic-beanstalk-application-descriptions-message-schema.json
slug: amazon-elastic-beanstalk-application-descriptions-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-application-descriptions-message-schema.json\",\n  \"title\": \"ApplicationDescriptionsMessage\",\n  \"description\": \"ApplicationDescriptionsMessage schema from Amazon Elastic Beanstalk AWS Elastic Beanstalk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApplicationDescription\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-application-descriptions-message-schema.json
tags:
- Amazon Web Services
- AWS
- Auto Scaling
- Deployment
- Elastic Beanstalk
- PaaS
- Platform As A Service
- Web Applications
title: ApplicationDescriptionsMessage
---
