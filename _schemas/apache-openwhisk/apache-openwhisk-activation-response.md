---
description: ActivationResponse schema from Apache OpenWhisk
layout: schema
name: ActivationResponse
properties_list:
- description: Activation status
  name: status
  type: string
- description: HTTP status code equivalent
  name: statusCode
  type: integer
- description: ''
  name: success
  type: boolean
- description: Action result payload
  name: result
  type: object
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-activation-response-schema.json
slug: apache-openwhisk-activation-response
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActivationResponse
---
