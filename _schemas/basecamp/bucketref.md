---
description: Reference to the project (bucket) that contains a resource
layout: schema
name: BucketRef
properties_list:
- description: Project ID
  name: id
  type: integer
- description: Project name
  name: name
  type: string
- description: Resource type, always "Project"
  name: type
  type: string
- description: API URL for the project
  name: url
  type: string
- description: Web URL for the project
  name: app_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/bucketref-schema.json
slug: bucketref
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: BucketRef
---
