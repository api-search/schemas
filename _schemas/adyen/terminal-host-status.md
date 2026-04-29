---
description: Indicate the reachability of the host by the POI Terminal. State of a Host.
layout: schema
name: HostStatus
properties_list:
- description: Identification of the Acquirer.
  name: AcquirerID
  type: integer
- description: Indicate if a Host is reachable.
  name: IsReachableFlag
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-host-status-schema.json
slug: terminal-host-status
source_filename: terminal-host-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-host-status-schema.json\",\n  \"title\": \"HostStatus\",\n  \"description\": \"Indicate the reachability of the host by the POI Terminal. State of a Host.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcquirerID\": {\n      \"type\": \"integer\",\n      \"description\": \"Identification of the Acquirer.\"\n    },\n    \"IsReachableFlag\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Indicate if a Host is reachable.\"\n    }\n  },\n  \"required\": [\n    \"AcquirerID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-host-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: HostStatus
---
