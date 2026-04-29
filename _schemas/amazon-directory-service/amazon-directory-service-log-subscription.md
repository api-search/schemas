---
description: Represents a log subscription, which tracks real-time data from a chosen log group to a specified destination.
layout: schema
name: LogSubscription
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: LogGroupName
  type: object
- description: ''
  name: SubscriptionCreatedDateTime
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-log-subscription-schema.json
slug: amazon-directory-service-log-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-log-subscription-schema.json\",\n  \"title\": \"LogSubscription\",\n  \"description\": \"Represents a log subscription, which tracks real-time data from a chosen log group to a specified destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"Identifier (ID) of the directory that you want to associate with the log subscription.\"\n        }\n      ]\n    },\n    \"LogGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupName\"\n        },\n        {\n          \"description\": \"The name of the log group.\"\n        }\n      ]\n    },\n    \"SubscriptionCreatedDateTime\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubscriptionCreatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the log subscription was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-log-subscription-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: LogSubscription
---
