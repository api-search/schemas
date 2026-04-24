---
description: ''
layout: schema
name: Subscription
properties_list:
- description: Whether the authenticated user is subscribed
  name: subscribed
  type: boolean
- description: Total number of subscribers
  name: count
  type: integer
- description: API URL for this subscription resource
  name: url
  type: string
- description: List of subscribed people
  name: subscribers
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/subscription-schema.json
slug: subscription
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Subscription
---
