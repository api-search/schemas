---
description: NamespaceLimits schema from Apache OpenWhisk
layout: schema
name: NamespaceLimits
properties_list:
- description: Maximum concurrent activations
  name: concurrency
  type: integer
- description: Actions per minute limit
  name: minuteRate
  type: integer
- description: Actions per hour limit
  name: hourRate
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-namespace-limits-schema.json
slug: apache-openwhisk-namespace-limits
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: NamespaceLimits
---
