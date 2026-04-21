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
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: AsyncJobResponse
---
