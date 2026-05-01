---
description: TestAvailabilityConfigurationResponse schema from Amazon WorkMail API
layout: schema
name: TestAvailabilityConfigurationResponse
properties_list:
- description: ''
  name: TestPassed
  type: object
- description: ''
  name: FailureReason
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-test-availability-configuration-response-schema.json
slug: workmail-test-availability-configuration-response
source_filename: workmail-test-availability-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TestPassed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Boolean indicating whether the test passed or failed.\"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"String containing the reason for a failed test if <code>TestPassed</code> is false.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TestAvailabilityConfigurationResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-test-availability-configuration-response-schema.json\",\n  \"description\": \"TestAvailabilityConfigurationResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-test-availability-configuration-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: TestAvailabilityConfigurationResponse
---
