---
description: JobState schema from Amazon Snow Family API
layout: schema
name: JobState
properties_list: []
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-job-state-schema.json
slug: amazon-snow-family-job-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-state-schema.json\",\n  \"title\": \"JobState\",\n  \"description\": \"JobState schema from Amazon Snow Family API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"New\",\n    \"PreparingAppliance\",\n    \"PreparingShipment\",\n    \"InTransitToCustomer\",\n    \"WithCustomer\",\n    \"InTransitToAWS\",\n    \"WithAWSSortingFacility\",\n    \"WithAWS\",\n    \"InProgress\",\n    \"Complete\",\n    \"Cancelled\",\n    \"Listing\",\n    \"Pending\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-state-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: JobState
---
