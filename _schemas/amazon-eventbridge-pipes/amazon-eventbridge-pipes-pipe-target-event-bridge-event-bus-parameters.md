---
description: The parameters for using an EventBridge event bus as a target.
layout: schema
name: PipeTargetEventBridgeEventBusParameters
properties_list:
- description: ''
  name: DetailType
  type: object
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: Resources
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: Time
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-event-bridge-event-bus-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-event-bridge-event-bus-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-event-bridge-event-bus-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-event-bridge-event-bus-parameters-schema.json\",\n  \"title\": \"PipeTargetEventBridgeEventBusParameters\",\n  \"description\": \"The parameters for using an EventBridge event bus as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DetailType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventBridgeDetailType\"\n        },\n        {\n          \"description\": \"A free-form string, with a maximum of 128 characters, used to decide what fields to expect in the event detail.\"\n        }\n      ]\n    },\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventBridgeEndpointId\"\n        },\n        {\n          \"description\": \"<p>The URL subdomain of the endpoint.\
  \ For example, if the URL for Endpoint is https://abcde.veo.endpoints.event.amazonaws.com, then the EndpointId is <code>abcde.veo</code>.</p> <important> <p>When using Java, you must include <code>auth-crt</code> on the class path.</p> </important>\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventBridgeEventResourceList\"\n        },\n        {\n          \"description\": \"Amazon Web Services resources, identified by Amazon Resource Name (ARN), which the event primarily concerns. Any number, including zero, may be present.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventBridgeEventSource\"\n        },\n        {\n          \"description\": \"The source of the event.\"\n        }\n      ]\n    },\n    \"Time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonPath\"\n        },\n        {\n  \
  \        \"description\": \"The time stamp of the event, per <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339.txt\\\">RFC3339</a>. If no time stamp is provided, the time stamp of the <a href=\\\"https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_PutEvents.html\\\">PutEvents</a> call is used.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-event-bridge-event-bus-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetEventBridgeEventBusParameters
---
