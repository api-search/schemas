---
description: Corresponds to SCTE-35 segmentation_descriptor.
layout: schema
name: Scte35SegmentationDescriptor
properties_list:
- description: ''
  name: DeliveryRestrictions
  type: object
- description: ''
  name: SegmentNum
  type: object
- description: ''
  name: SegmentationCancelIndicator
  type: object
- description: ''
  name: SegmentationDuration
  type: object
- description: ''
  name: SegmentationEventId
  type: object
- description: ''
  name: SegmentationTypeId
  type: object
- description: ''
  name: SegmentationUpid
  type: object
- description: ''
  name: SegmentationUpidType
  type: object
- description: ''
  name: SegmentsExpected
  type: object
- description: ''
  name: SubSegmentNum
  type: object
- description: ''
  name: SubSegmentsExpected
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-segmentation-descriptor-schema.json
slug: medialive-api-scte35-segmentation-descriptor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-segmentation-descriptor-schema.json\",\n  \"title\": \"Scte35SegmentationDescriptor\",\n  \"description\": \"Corresponds to SCTE-35 segmentation_descriptor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryRestrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35DeliveryRestrictions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deliveryRestrictions\"\n          },\n          \"description\": \"Holds the four SCTE-35 delivery restriction parameters.\"\n        }\n      ]\n    },\n    \"SegmentNum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentNum\"\n          },\n      \
  \    \"description\": \"Corresponds to SCTE-35 segment_num. A value that is valid for the specified segmentation_type_id.\"\n        }\n      ]\n    },\n    \"SegmentationCancelIndicator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35SegmentationCancelIndicator\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationCancelIndicator\"\n          },\n          \"description\": \"Corresponds to SCTE-35 segmentation_event_cancel_indicator.\"\n        }\n      ]\n    },\n    \"SegmentationDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__longMin0Max1099511627775\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationDuration\"\n          },\n          \"description\": \"Corresponds to SCTE-35 segmentation_duration. Optional. The duration for the time_signal, in 90 KHz ticks. To convert seconds to ticks, multiple the seconds by 90,000. Enter time in 90 KHz\
  \ clock ticks. If you do not enter a duration, the time_signal will continue until you insert a cancellation message.\"\n        }\n      ]\n    },\n    \"SegmentationEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__longMin0Max4294967295\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationEventId\"\n          },\n          \"description\": \"Corresponds to SCTE-35 segmentation_event_id. \"\n        }\n      ]\n    },\n    \"SegmentationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationTypeId\"\n          },\n          \"description\": \"Corresponds to SCTE-35 segmentation_type_id. One of the segmentation_type_id values listed in the SCTE-35 specification. On the console, enter the ID in decimal (for example, \\\"52\\\"). In the CLI, API, or an SDK, enter the ID in hex (for example,\
  \ \\\"0x34\\\") or decimal (for example, \\\"52\\\").\"\n        }\n      ]\n    },\n    \"SegmentationUpid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationUpid\"\n          },\n          \"description\": \"Corresponds to SCTE-35 segmentation_upid. Enter a string containing the hexadecimal representation of the characters that make up the SCTE-35 segmentation_upid value. Must contain an even number of hex characters. Do not include spaces between each hex pair. For example, the ASCII \\\"ADS Information\\\" becomes hex \\\"41445320496e666f726d6174696f6e.\"\n        }\n      ]\n    },\n    \"SegmentationUpidType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationUpidType\"\n          },\n          \"description\": \"Corresponds to SCTE-35\
  \ segmentation_upid_type. On the console, enter one of the types listed in the SCTE-35 specification, converted to a decimal. For example, \\\"0x0C\\\" hex from the specification is \\\"12\\\" in decimal. In the CLI, API, or an SDK, enter one of the types listed in the SCTE-35 specification, in either hex (for example, \\\"0x0C\\\" ) or in decimal (for example, \\\"12\\\").\"\n        }\n      ]\n    },\n    \"SegmentsExpected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentsExpected\"\n          },\n          \"description\": \"Corresponds to SCTE-35 segments_expected. A value that is valid for the specified segmentation_type_id.\"\n        }\n      ]\n    },\n    \"SubSegmentNum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subSegmentNum\"\
  \n          },\n          \"description\": \"Corresponds to SCTE-35 sub_segment_num. A value that is valid for the specified segmentation_type_id.\"\n        }\n      ]\n    },\n    \"SubSegmentsExpected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subSegmentsExpected\"\n          },\n          \"description\": \"Corresponds to SCTE-35 sub_segments_expected. A value that is valid for the specified segmentation_type_id.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SegmentationEventId\",\n    \"SegmentationCancelIndicator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-segmentation-descriptor-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte35SegmentationDescriptor
---
