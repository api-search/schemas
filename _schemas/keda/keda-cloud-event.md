---
description: Schema for CloudEvents emitted by KEDA when scaling-related events occur. Events follow the CloudEvents specification v1.0 and are delivered to HTTP or Azure Event Grid destinations configured in a CloudEventSource or ClusterCloudEventSource resource.
layout: schema
name: KEDA CloudEvent
properties_list:
- description: CloudEvents specification version. Always 1.0 for KEDA events.
  name: specversion
  type: string
- description: CloudEvent type identifier. Always com.cloudeventsource.keda for events emitted by KEDA.
  name: type
  type: string
- description: URI identifying the KEDA instance that emitted the event, in the format /{cluster-name}/{keda-namespace}/keda.
  name: source
  type: string
- description: URI identifying the specific resource that triggered the event, in the format /{cluster-name}/{namespace}/{object-type}/{object-name}.
  name: subject
  type: string
- description: Unique identifier for this CloudEvent instance.
  name: id
  type: string
- description: ISO 8601 timestamp of when the event was emitted.
  name: time
  type: string
- description: MIME type of the data field. Always application/json.
  name: datacontenttype
  type: string
- description: ''
  name: data
  type: object
provider_name: KEDA
provider_slug: keda
schema_file: json-schema/keda-cloud-event-schema.json
slug: keda-cloud-event
source_filename: keda-cloud-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://keda.sh/schemas/keda/cloud-event.json\",\n  \"title\": \"KEDA CloudEvent\",\n  \"description\": \"Schema for CloudEvents emitted by KEDA when scaling-related events occur. Events follow the CloudEvents specification v1.0 and are delivered to HTTP or Azure Event Grid destinations configured in a CloudEventSource or ClusterCloudEventSource resource.\",\n  \"type\": \"object\",\n  \"required\": [\"specversion\", \"type\", \"source\", \"subject\", \"id\", \"time\", \"datacontenttype\", \"data\"],\n  \"properties\": {\n    \"specversion\": {\n      \"type\": \"string\",\n      \"const\": \"1.0\",\n      \"description\": \"CloudEvents specification version. Always 1.0 for KEDA events.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"com.cloudeventsource.keda\",\n      \"description\": \"CloudEvent type identifier. Always com.cloudeventsource.keda for events emitted\
  \ by KEDA.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"pattern\": \"^/[^/]*/[^/]*/keda$\",\n      \"description\": \"URI identifying the KEDA instance that emitted the event, in the format /{cluster-name}/{keda-namespace}/keda.\",\n      \"example\": \"/my-cluster/keda/keda\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"pattern\": \"^/[^/]*/[^/]*/[^/]*/[^/]*$\",\n      \"description\": \"URI identifying the specific resource that triggered the event, in the format /{cluster-name}/{namespace}/{object-type}/{object-name}.\",\n      \"example\": \"/my-cluster/default/scaledobject/my-app-scaler\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for this CloudEvent instance.\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when\
  \ the event was emitted.\",\n      \"example\": \"2026-03-18T10:00:00Z\"\n    },\n    \"datacontenttype\": {\n      \"type\": \"string\",\n      \"const\": \"application/json\",\n      \"description\": \"MIME type of the data field. Always application/json.\"\n    },\n    \"data\": {\n      \"$ref\": \"#/$defs/EventData\"\n    }\n  },\n  \"$defs\": {\n    \"EventData\": {\n      \"type\": \"object\",\n      \"description\": \"Payload data carried by a KEDA CloudEvent, providing machine-readable reason code and human-readable detail message.\",\n      \"required\": [\"reason\", \"message\"],\n      \"properties\": {\n        \"reason\": {\n          \"type\": \"string\",\n          \"description\": \"Machine-readable reason code identifying the type of scaling event that occurred.\",\n          \"enum\": [\n            \"ScalerError\",\n            \"ScaledObjectReady\",\n            \"ScaledObjectDeleted\",\n            \"ScaledJobReady\",\n            \"ScaledJobDeleted\",\n         \
  \   \"KEDAScalersStarted\",\n            \"KEDAScalersStopped\",\n            \"AuthenticationFailed\"\n          ],\n          \"example\": \"ScalerError\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description providing context about the scaling event, including which resource was affected and any error details.\",\n          \"example\": \"Error when getting metric for trigger type kafka. Unable to connect to broker at kafka-broker:9092\"\n        }\n      }\n    },\n    \"CloudEventSource\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes custom resource that configures where KEDA delivers CloudEvents. CloudEventSource is namespace-scoped; ClusterCloudEventSource is cluster-scoped.\",\n      \"required\": [\"apiVersion\", \"kind\", \"metadata\", \"spec\"],\n      \"properties\": {\n        \"apiVersion\": {\n          \"type\": \"string\",\n          \"const\": \"eventing.keda.sh/v1alpha1\",\n\
  \          \"description\": \"API version for the KEDA CloudEventSource resource.\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"enum\": [\"CloudEventSource\", \"ClusterCloudEventSource\"],\n          \"description\": \"Resource kind. CloudEventSource is namespace-scoped; ClusterCloudEventSource applies cluster-wide.\"\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Standard Kubernetes object metadata.\",\n          \"required\": [\"name\"],\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Name of the CloudEventSource resource.\"\n            },\n            \"namespace\": {\n              \"type\": \"string\",\n              \"description\": \"Namespace (CloudEventSource only).\"\n            }\n          }\n        },\n        \"spec\": {\n          \"$ref\": \"#/$defs/CloudEventSourceSpec\"\n        }\n      }\n    },\n   \
  \ \"CloudEventSourceSpec\": {\n      \"type\": \"object\",\n      \"description\": \"Specification for a CloudEventSource defining the destination and optional event type filters.\",\n      \"required\": [\"destination\"],\n      \"properties\": {\n        \"clusterName\": {\n          \"type\": \"string\",\n          \"description\": \"Optional cluster name included in the CloudEvent source and subject fields. Defaults to the Kubernetes cluster name if discoverable.\"\n        },\n        \"authenticationRef\": {\n          \"type\": \"object\",\n          \"description\": \"Optional reference to a TriggerAuthentication for authenticating CloudEvent delivery to the destination.\",\n          \"required\": [\"name\"],\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Name of the TriggerAuthentication resource.\"\n            },\n            \"kind\": {\n              \"type\": \"string\",\n              \"enum\"\
  : [\"TriggerAuthentication\", \"ClusterTriggerAuthentication\"],\n              \"description\": \"Kind of the authentication resource.\"\n            }\n          }\n        },\n        \"destination\": {\n          \"$ref\": \"#/$defs/CloudEventDestination\"\n        },\n        \"eventSubscription\": {\n          \"$ref\": \"#/$defs/EventSubscription\"\n        }\n      }\n    },\n    \"CloudEventDestination\": {\n      \"type\": \"object\",\n      \"description\": \"Destination configuration for CloudEvent delivery. Either an HTTP endpoint or Azure Event Grid topic must be configured.\",\n      \"properties\": {\n        \"http\": {\n          \"type\": \"object\",\n          \"description\": \"HTTP destination configuration for CloudEvent delivery.\",\n          \"required\": [\"uri\"],\n          \"properties\": {\n            \"uri\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"HTTP(S) URL to which KEDA will POST CloudEvents.\"\
  ,\n              \"example\": \"https://my-sink.example.com/events\"\n            }\n          }\n        },\n        \"azureEventGridTopic\": {\n          \"type\": \"object\",\n          \"description\": \"Azure Event Grid destination configuration for CloudEvent delivery.\",\n          \"required\": [\"endpoint\"],\n          \"properties\": {\n            \"endpoint\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"Azure Event Grid topic endpoint URL.\",\n              \"example\": \"https://my-topic.eventgrid.azure.net/api/events\"\n            }\n          }\n        }\n      }\n    },\n    \"EventSubscription\": {\n      \"type\": \"object\",\n      \"description\": \"Optional event type filter configuration for the CloudEventSource.\",\n      \"properties\": {\n        \"includedEventTypes\": {\n          \"type\": \"array\",\n          \"description\": \"When specified, only events with these reason codes are delivered.\
  \ All others are suppressed.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"keda.scaledobject.ready.v1\",\n              \"keda.scaledobject.removed.v1\",\n              \"keda.scaledobject.failed.v1\",\n              \"keda.scaledjob.ready.v1\",\n              \"keda.scaledjob.removed.v1\",\n              \"keda.scaledjob.failed.v1\"\n            ]\n          }\n        },\n        \"excludedEventTypes\": {\n          \"type\": \"array\",\n          \"description\": \"Events with these reason codes are suppressed and not delivered.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"keda.scaledobject.ready.v1\",\n              \"keda.scaledobject.removed.v1\",\n              \"keda.scaledobject.failed.v1\",\n              \"keda.scaledjob.ready.v1\",\n              \"keda.scaledjob.removed.v1\",\n              \"keda.scaledjob.failed.v1\"\n            ]\n          }\n        }\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/json-schema/keda-cloud-event-schema.json
tags:
- Autoscaling
- CNCF
- Event-Driven
- Graduated
- Kubernetes
title: KEDA CloudEvent
---
