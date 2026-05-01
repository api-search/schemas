---
description: Corresponds to SCTE-35 segmentation_event_cancel_indicator. SEGMENTATION_EVENT_NOT_CANCELED corresponds to 0 in the SCTE-35 specification and indicates that this is an insertion request. SEGMENTATION_EVENT_CANCELED corresponds to 1 in the SCTE-35 specification and indicates that this is a cancelation request, in which case complete this field and the existing event ID to cancel.
layout: schema
name: Scte35SegmentationCancelIndicator
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-segmentation-cancel-indicator-schema.json
slug: medialive-api-scte35-segmentation-cancel-indicator
source_filename: medialive-api-scte35-segmentation-cancel-indicator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-segmentation-cancel-indicator-schema.json\",\n  \"title\": \"Scte35SegmentationCancelIndicator\",\n  \"description\": \"Corresponds to SCTE-35 segmentation_event_cancel_indicator. SEGMENTATION_EVENT_NOT_CANCELED corresponds to 0 in the SCTE-35 specification and indicates that this is an insertion request. SEGMENTATION_EVENT_CANCELED corresponds to 1 in the SCTE-35 specification and indicates that this is a cancelation request, in which case complete this field and the existing event ID to cancel.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SEGMENTATION_EVENT_NOT_CANCELED\",\n    \"SEGMENTATION_EVENT_CANCELED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-segmentation-cancel-indicator-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35SegmentationCancelIndicator
---
