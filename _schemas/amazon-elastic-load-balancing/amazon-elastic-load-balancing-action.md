---
description: Describes an action for a listener or rule
layout: schema
name: Action
properties_list:
- description: The type of action
  name: type
  type: string
- description: The ARN of the target group for forward actions
  name: targetGroupArn
  type: string
- description: The order for the action
  name: order
  type: integer
- description: Configuration for redirect actions
  name: redirectConfig
  type: object
- description: Configuration for fixed-response actions
  name: fixedResponseConfig
  type: object
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-action-schema.json
slug: amazon-elastic-load-balancing-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"Describes an action for a listener or rule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of action\",\n      \"enum\": [\n        \"forward\",\n        \"authenticate-oidc\",\n        \"authenticate-cognito\",\n        \"redirect\",\n        \"fixed-response\"\n      ]\n    },\n    \"targetGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the target group for forward actions\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"The order for the action\"\n    },\n    \"redirectConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration\
  \ for redirect actions\",\n      \"properties\": {\n        \"protocol\": {\n          \"type\": \"string\",\n          \"description\": \"The protocol\"\n        },\n        \"port\": {\n          \"type\": \"string\",\n          \"description\": \"The port\"\n        },\n        \"host\": {\n          \"type\": \"string\",\n          \"description\": \"The hostname\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"The absolute path\"\n        },\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"The query parameters\"\n        },\n        \"statusCode\": {\n          \"type\": \"string\",\n          \"description\": \"The HTTP redirect code\",\n          \"enum\": [\n            \"HTTP_301\",\n            \"HTTP_302\"\n          ]\n        }\n      }\n    },\n    \"fixedResponseConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for fixed-response actions\",\n      \"properties\"\
  : {\n        \"messageBody\": {\n          \"type\": \"string\",\n          \"description\": \"The message body\"\n        },\n        \"statusCode\": {\n          \"type\": \"string\",\n          \"description\": \"The HTTP response code\"\n        },\n        \"contentType\": {\n          \"type\": \"string\",\n          \"description\": \"The content type\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-action-schema.json
tags:
- Amazon Web Services
- AWS
- High Availability
- Load Balancing
- Networking
- Scalability
title: Action
---
