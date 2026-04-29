---
description: ListAvailabilityConfigurationsResponse schema from Amazon WorkMail API
layout: schema
name: ListAvailabilityConfigurationsResponse
properties_list:
- description: ''
  name: AvailabilityConfigurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-availability-configurations-response-schema.json
slug: workmail-list-availability-configurations-response
source_filename: workmail-list-availability-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityConfigurationList\"\n        },\n        {\n          \"description\": \"The list of <code>AvailabilityConfiguration</code>'s that exist for the specified WorkMail organization.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The value is <code>null</code> when there are no further results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListAvailabilityConfigurationsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-availability-configurations-response-schema.json\"\
  ,\n  \"description\": \"ListAvailabilityConfigurationsResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-availability-configurations-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListAvailabilityConfigurationsResponse
---
