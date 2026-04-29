---
description: EmailConfigurations schema
layout: schema
name: EmailConfigurations
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-email-configurations-schema.json
slug: iot-events-email-configurations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-email-configurations-schema.json\",\n  \"title\": \"EmailConfigurations\",\n  \"description\": \"EmailConfigurations schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"from\",\n      \"recipients\"\n    ],\n    \"properties\": {\n      \"from\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FromEmail\"\n          },\n          {\n            \"description\": \"<p>The email address that sends emails.</p> <important> <p>If you use the AWS IoT Events managed AWS Lambda function to manage your emails, you must <a href=\\\"https://docs.aws.amazon.com/ses/latest/DeveloperGuide/verify-email-addresses.html\\\">verify the email address that sends emails in Amazon SES</a>.</p> </important>\"\n          }\n \
  \       ]\n      },\n      \"content\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EmailContent\"\n          },\n          {\n            \"description\": \"Contains the subject and message of an email.\"\n          }\n        ]\n      },\n      \"recipients\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EmailRecipients\"\n          },\n          {\n            \"description\": \"<p>Contains the information of one or more recipients who receive the emails.</p> <important> <p>You must <a href=\\\"https://docs.aws.amazon.com/singlesignon/latest/userguide/addusers.html\\\">add the users that receive emails to your AWS SSO store</a>.</p> </important>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains the configuration information of email notifications.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-email-configurations-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: EmailConfigurations
---
