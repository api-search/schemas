---
description: The name of an Availability Zone for use during database migration. <code>AvailabilityZone</code> is an optional parameter to the <a href="https://docs.aws.amazon.com/dms/latest/APIReference/API_CreateReplicationInstance.html"> <code>CreateReplicationInstance</code> </a> operation, and it’s value relates to the Amazon Web Services Region of an endpoint. For example, the availability zone of an endpoint in the us-east-1 region might be us-east-1a, us-east-1b, us-east-1c, or us-east-1d.
layout: schema
name: AvailabilityZone
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-availability-zone-schema.json
slug: amazon-dms-availability-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-availability-zone-schema.json\",\n  \"title\": \"AvailabilityZone\",\n  \"description\": \"The name of an Availability Zone for use during database migration. <code>AvailabilityZone</code> is an optional parameter to the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_CreateReplicationInstance.html\\\"> <code>CreateReplicationInstance</code> </a> operation, and it\\u2019s value relates to the Amazon Web Services Region of an endpoint. For example, the availability zone of an endpoint in the us-east-1 region might be us-east-1a, us-east-1b, us-east-1c, or us-east-1d.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of\
  \ the Availability Zone.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-availability-zone-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: AvailabilityZone
---
