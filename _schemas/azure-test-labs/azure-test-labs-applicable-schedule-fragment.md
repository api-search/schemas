---
description: Schedules applicable to a virtual machine. The schedules may have been defined on a VM or on lab level.
layout: schema
name: ApplicableScheduleFragment
properties_list:
- description: The properties of the resource.
  name: properties
  type: object
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-applicable-schedule-fragment-schema.json
slug: azure-test-labs-applicable-schedule-fragment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-applicable-schedule-fragment-schema.json\",\n  \"title\": \"ApplicableScheduleFragment\",\n  \"description\": \"Schedules applicable to a virtual machine. The schedules may have been defined on a VM or on lab level.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ApplicableSchedulePropertiesFragment\",\n      \"description\": \"The properties of the resource.\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-applicable-schedule-fragment-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ApplicableScheduleFragment
---
