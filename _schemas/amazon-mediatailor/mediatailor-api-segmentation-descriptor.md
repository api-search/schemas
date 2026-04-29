---
description: <p>The <code>segmentation_descriptor</code> message can contain advanced metadata fields, like content identifiers, to convey a wide range of information about the ad break. MediaTailor writes the ad metadata in the egress manifest as part of the <code>EXT-X-DATERANGE</code> or <code>EventStream</code> ad marker's SCTE-35 data.</p> <p> <code>segmentation_descriptor</code> messages must be sent with the <code>time_signal</code> message type.</p> <p>See the <code>segmentation_descriptor()</code> table of the 2022 SCTE-35 specification for more information.</p>
layout: schema
name: SegmentationDescriptor
properties_list:
- description: ''
  name: SegmentNum
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
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-segmentation-descriptor-schema.json
slug: mediatailor-api-segmentation-descriptor
source_filename: mediatailor-api-segmentation-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-segmentation-descriptor-schema.json\",\n  \"title\": \"SegmentationDescriptor\",\n  \"description\": \"<p>The <code>segmentation_descriptor</code> message can contain advanced metadata fields, like content identifiers, to convey a wide range of information about the ad break. MediaTailor writes the ad metadata in the egress manifest as part of the <code>EXT-X-DATERANGE</code> or <code>EventStream</code> ad marker's SCTE-35 data.</p> <p> <code>segmentation_descriptor</code> messages must be sent with the <code>time_signal</code> message type.</p> <p>See the <code>segmentation_descriptor()</code> table of the 2022 SCTE-35 specification for more information.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SegmentNum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The segment number to assign to the <code>segmentation_descriptor.segment_num</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification Values must be between 0 and 256, inclusive. The default value is 0.\"\n        }\n      ]\n    },\n    \"SegmentationEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The Event Identifier to assign to the <code>segmentation_descriptor.segmentation_event_id</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification. The default value is 1.\"\n        }\n      ]\n    },\n    \"SegmentationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The Type Identifier to assign to the <code>segmentation_descriptor.segmentation_type_id</code>\
  \ message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification. Values must be between 0 and 256, inclusive. The default value is 48.\"\n        }\n      ]\n    },\n    \"SegmentationUpid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Upid to assign to the <code>segmentation_descriptor.segmentation_upid</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification. The value must be a hexadecimal string containing only the characters 0 though 9 and A through F. The default value is \\\"\\\" (an empty string).\"\n        }\n      ]\n    },\n    \"SegmentationUpidType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The Upid Type to assign to the <code>segmentation_descriptor.segmentation_upid_type</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification.\
  \ Values must be between 0 and 256, inclusive. The default value is 14.\"\n        }\n      ]\n    },\n    \"SegmentsExpected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of segments expected, which is assigned to the <code>segmentation_descriptor.segments_expectedS</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification Values must be between 0 and 256, inclusive. The default value is 0.\"\n        }\n      ]\n    },\n    \"SubSegmentNum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The sub-segment number to assign to the <code>segmentation_descriptor.sub_segment_num</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification. Values must be between 0 and 256, inclusive. The defualt value is null.\"\n        }\n      ]\n    },\n    \"SubSegmentsExpected\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of sub-segments expected, which is assigned to the <code>segmentation_descriptor.sub_segments_expected</code> message, as defined in section 10.3.3.1 of the 2022 SCTE-35 specification. Values must be between 0 and 256, inclusive. The default value is null.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-segmentation-descriptor-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SegmentationDescriptor
---
