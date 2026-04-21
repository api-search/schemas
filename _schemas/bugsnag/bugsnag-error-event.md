---
description: Represents an individual error event reported to or retrieved from Bugsnag, containing exception details, stack traces, device and application information, breadcrumbs, and custom metadata.
layout: schema
name: Bugsnag Error Event
properties_list:
- description: The list of exceptions that occurred. The first exception is the most significant. Multiple exceptions represent a causal chain.
  name: exceptions
  type: array
- description: A trail of events leading up to the error, providing context about user actions and application state.
  name: breadcrumbs
  type: array
- description: ''
  name: request
  type: object
- description: Information about all running threads at the time of the error.
  name: threads
  type: array
- description: A string representing what was happening in the application at the time of the error, such as a controller action or route name.
  name: context
  type: string
- description: A custom grouping hash to override default error grouping. Events with the same hash are grouped together.
  name: groupingHash
  type: string
- description: Whether this error was unhandled (true) or caught and handled (false) by the application.
  name: unhandled
  type: boolean
- description: The severity level of the error.
  name: severity
  type: string
- description: ''
  name: severityReason
  type: object
- description: ''
  name: user
  type: object
- description: ''
  name: app
  type: object
- description: ''
  name: device
  type: object
- description: ''
  name: session
  type: object
- description: Custom metadata organized by tab name. Each key represents a tab on the Bugsnag dashboard containing key-value debugging information.
  name: metaData
  type: object
provider_name: bugsnag
provider_slug: bugsnag
schema_file: json-schema/bugsnag-error-event-schema.json
slug: bugsnag-error-event
tags: []
title: Bugsnag Error Event
---
