---
description: Response returned when an asynchronous CloudStack API operation is initiated.
layout: schema
name: AsyncJobResponse
properties_list:
- description: UUID of the asynchronous job to poll for completion.
  name: jobid
  type: string
- description: UUID of the resource being created or modified.
  name: id
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-async-job-response-schema.json
slug: cloudstack-api-async-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-async-job-response-schema.json\",\n  \"title\": \"AsyncJobResponse\",\n  \"description\": \"Response returned when an asynchronous CloudStack API operation is initiated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobid\": { \"type\": \"string\", \"description\": \"UUID of the asynchronous job to poll for completion.\", \"example\": \"a4b6c8d0-1234-5678-90ab-cdef01234567\" },\n    \"id\": { \"type\": \"string\", \"description\": \"UUID of the resource being created or modified.\", \"example\": \"vm-uuid-1234\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-async-job-response-schema.json
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: AsyncJobResponse
---
