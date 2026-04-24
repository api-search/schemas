---
description: ''
layout: schema
name: ProjectAccessRequest
properties_list:
- description: Array of person IDs to grant access
  name: grant
  type: array
- description: Array of person IDs to revoke access
  name: revoke
  type: array
- description: New people to invite to the project
  name: create
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectaccessrequest-schema.json
slug: projectaccessrequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectAccessRequest
---
