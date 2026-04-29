---
description: Properties of a schedules applicable to a virtual machine.
layout: schema
name: ApplicableScheduleProperties
properties_list:
- description: The auto-shutdown schedule, if one has been set at the lab or lab resource level.
  name: labVmsShutdown
  type: object
- description: The auto-startup schedule, if one has been set at the lab or lab resource level.
  name: labVmsStartup
  type: object
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-applicable-schedule-properties-schema.json
slug: azure-test-labs-applicable-schedule-properties
source_filename: azure-test-labs-applicable-schedule-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-applicable-schedule-properties-schema.json\",\n  \"title\": \"ApplicableScheduleProperties\",\n  \"description\": \"Properties of a schedules applicable to a virtual machine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"labVmsShutdown\": {\n      \"$ref\": \"#/definitions/Schedule\",\n      \"description\": \"The auto-shutdown schedule, if one has been set at the lab or lab resource level.\"\n    },\n    \"labVmsStartup\": {\n      \"$ref\": \"#/definitions/Schedule\",\n      \"description\": \"The auto-startup schedule, if one has been set at the lab or lab resource level.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-applicable-schedule-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ApplicableScheduleProperties
---
