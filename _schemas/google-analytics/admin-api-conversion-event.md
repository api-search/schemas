---
description: A conversion event in a Google Analytics property.
layout: schema
name: ConversionEvent
properties_list:
- description: Optional. The method by which conversions will be counted across multiple events within a session. If this value is not provided, it will be set to `ONCE_PER_EVENT`.
  name: countingMethod
  type: string
- description: Output only. Time when this conversion event was created in the property.
  name: createTime
  type: string
- description: Output only. If set to true, this conversion event refers to a custom event. If set to false, this conversion event refers to a default event in GA. Default events typically have special meaning in GA
  name: custom
  type: boolean
- description: Defines a default value/currency for a conversion event. Both value and currency must be provided.
  name: defaultConversionValue
  type: object
- description: Output only. If set, this event can currently be deleted with DeleteConversionEvent.
  name: deletable
  type: boolean
- description: 'Immutable. The event name for this conversion event. Examples: ''click'', ''purchase'''
  name: eventName
  type: string
- description: 'Output only. Resource name of this conversion event. Format: properties/{property}/conversionEvents/{conversion_event}'
  name: name
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-conversion-event-schema.json
slug: admin-api-conversion-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-conversion-event-schema.json\",\n  \"title\": \"ConversionEvent\",\n  \"description\": \"A conversion event in a Google Analytics property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countingMethod\": {\n      \"description\": \"Optional. The method by which conversions will be counted across multiple events within a session. If this value is not provided, it will be set to `ONCE_PER_EVENT`.\",\n      \"enum\": [\n        \"CONVERSION_COUNTING_METHOD_UNSPECIFIED\",\n        \"ONCE_PER_EVENT\",\n        \"ONCE_PER_SESSION\"\n      ],\n      \"type\": \"string\",\n      \"example\": \"CONVERSION_COUNTING_METHOD_UNSPECIFIED\"\n    },\n    \"createTime\": {\n      \"description\": \"Output only. Time when this conversion event was created in the property.\",\n      \"format\": \"google-datetime\"\
  ,\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"custom\": {\n      \"description\": \"Output only. If set to true, this conversion event refers to a custom event. If set to false, this conversion event refers to a default event in GA. Default events typically have special meaning in GA. Default events are usually created for you by the GA system, but in some cases can be created by property admins. Custom events count towards the maximum number of custom conversion events that may be created per property.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"defaultConversionValue\": {\n      \"description\": \"Defines a default value/currency for a conversion event. Both value and currency must be provided.\",\n      \"properties\": {\n        \"currencyCode\": {\n          \"description\": \"When a conversion event for this event_name has no set currency, this currency\
  \ will be applied as the default. Must be in ISO 4217 currency code format. See https://en.wikipedia.org/wiki/ISO_4217 for more information.\",\n          \"type\": \"string\"\n        },\n        \"value\": {\n          \"description\": \"This value will be used to populate the value for all conversions of the specified event_name where the event \\\"value\\\" parameter is unset.\",\n          \"format\": \"double\",\n          \"type\": \"number\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"deletable\": {\n      \"description\": \"Output only. If set, this event can currently be deleted with DeleteConversionEvent.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"eventName\": {\n      \"description\": \"Immutable. The event name for this conversion event. Examples: 'click', 'purchase'\",\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"name\": {\n      \"description\": \"Output only.\
  \ Resource name of this conversion event. Format: properties/{property}/conversionEvents/{conversion_event}\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-conversion-event-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: ConversionEvent
---
