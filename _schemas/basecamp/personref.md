---
description: Minimal reference to a Basecamp person
layout: schema
name: PersonRef
properties_list:
- description: Person ID
  name: id
  type: integer
- description: Signed global ID for attaching this person
  name: attachable_sgid
  type: string
- description: Full name
  name: name
  type: string
- description: Email address
  name: email_address
  type: string
- description: Type of personable (User, Client, etc.)
  name: personable_type
  type: string
- description: Job title
  name: title
  type: string
- description: Short biography
  name: bio
  type: string
- description: Location string
  name: location
  type: string
- description: Account creation timestamp
  name: created_at
  type: string
- description: Last update timestamp
  name: updated_at
  type: string
- description: Whether the person is an account administrator
  name: admin
  type: boolean
- description: Whether the person is the account owner
  name: owner
  type: boolean
- description: Whether the person is a client user
  name: client
  type: boolean
- description: Whether the person is an employee
  name: employee
  type: boolean
- description: IANA time zone name
  name: time_zone
  type: string
- description: URL to the person's avatar image
  name: avatar_url
  type: string
- description: Company the person belongs to
  name: company
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/personref-schema.json
slug: personref
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: PersonRef
---
