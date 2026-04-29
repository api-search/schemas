---
description: Options for VM migration during infrastructure maintenance on launch
layout: schema
name: LaunchInstanceAvailabilityConfigDetails
properties_list:
- description: Whether live migration is the preferred option
  name: isLiveMigrationPreferred
  type: boolean
- description: The lifecycle state for an instance when maintenance is due
  name: recoveryAction
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-launch-instance-availability-config-details-schema.json
slug: oci-compute-launch-instance-availability-config-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LaunchInstanceAvailabilityConfigDetails\",\n  \"type\": \"object\",\n  \"description\": \"Options for VM migration during infrastructure maintenance on launch\",\n  \"properties\": {\n    \"isLiveMigrationPreferred\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether live migration is the preferred option\"\n    },\n    \"recoveryAction\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state for an instance when maintenance is due\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-launch-instance-availability-config-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: LaunchInstanceAvailabilityConfigDetails
---
