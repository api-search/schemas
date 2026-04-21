---
description: An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, only values 1-99 would be matched.
layout: schema
name: MatchRange
properties_list:
- description: ''
  name: end
  type: object
- description: ''
  name: start
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-match-range-schema.json
slug: app-mesh-match-range
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: MatchRange
---
