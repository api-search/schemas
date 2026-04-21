---
description: Standard error response returned by the Apidog API when a request fails due to authentication issues, missing resources, or other problems.
layout: schema
name: Apidog Error
properties_list:
- description: Always false for error responses.
  name: success
  type: boolean
- description: Details about the error that occurred.
  name: error
  type: object
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-error-schema.json
slug: apidog-error
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Error
---
