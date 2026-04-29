---
description: Corresponds to the archive_allowed parameter. A value of ARCHIVE_NOT_ALLOWED corresponds to 0 (false) in the SCTE-35 specification. If you include one of the "restriction" flags then you must include all four of them.
layout: schema
name: Scte35ArchiveAllowedFlag
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-archive-allowed-flag-schema.json
slug: medialive-api-scte35-archive-allowed-flag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-archive-allowed-flag-schema.json\",\n  \"title\": \"Scte35ArchiveAllowedFlag\",\n  \"description\": \"Corresponds to the archive_allowed parameter. A value of ARCHIVE_NOT_ALLOWED corresponds to 0 (false) in the SCTE-35 specification. If you include one of the \\\"restriction\\\" flags then you must include all four of them.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ARCHIVE_NOT_ALLOWED\",\n    \"ARCHIVE_ALLOWED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-archive-allowed-flag-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte35ArchiveAllowedFlag
---
