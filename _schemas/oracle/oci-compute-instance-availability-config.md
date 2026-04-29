---
description: Options for VM migration during infrastructure maintenance
layout: schema
name: InstanceAvailabilityConfig
properties_list:
- description: Whether live migration is the preferred option during maintenance
  name: isLiveMigrationPreferred
  type: boolean
- description: The lifecycle state for an instance when maintenance is due
  name: recoveryAction
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-instance-availability-config-schema.json
slug: oci-compute-instance-availability-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceAvailabilityConfig\",\n  \"type\": \"object\",\n  \"description\": \"Options for VM migration during infrastructure maintenance\",\n  \"properties\": {\n    \"isLiveMigrationPreferred\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether live migration is the preferred option during maintenance\"\n    },\n    \"recoveryAction\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state for an instance when maintenance is due\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-instance-availability-config-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: InstanceAvailabilityConfig
---
