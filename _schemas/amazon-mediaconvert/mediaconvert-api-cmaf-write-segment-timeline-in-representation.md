---
description: When you enable Precise segment duration in DASH manifests (writeSegmentTimelineInRepresentation), your DASH manifest shows precise segment durations. The segment duration information appears inside the SegmentTimeline element, inside SegmentTemplate at the Representation level. When this feature isn't enabled, the segment durations in your DASH manifest are approximate. The segment duration information appears in the duration attribute of the SegmentTemplate element.
layout: schema
name: CmafWriteSegmentTimelineInRepresentation
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-write-segment-timeline-in-representation-schema.json
slug: mediaconvert-api-cmaf-write-segment-timeline-in-representation
source_filename: mediaconvert-api-cmaf-write-segment-timeline-in-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-write-segment-timeline-in-representation-schema.json\",\n  \"title\": \"CmafWriteSegmentTimelineInRepresentation\",\n  \"description\": \"When you enable Precise segment duration in DASH manifests (writeSegmentTimelineInRepresentation), your DASH manifest shows precise segment durations. The segment duration information appears inside the SegmentTimeline element, inside SegmentTemplate at the Representation level. When this feature isn't enabled, the segment durations in your DASH manifest are approximate. The segment duration information appears in the duration attribute of the SegmentTemplate element.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENABLED\",\n    \"DISABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-write-segment-timeline-in-representation-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CmafWriteSegmentTimelineInRepresentation
---
