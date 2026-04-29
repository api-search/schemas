---
description: 'Flight code-share status<p>Possible values:</p> <ul> <li><b>0 - Unknown</b>: Code-sharing information is unavailable for this flight. Flight might be operated both by airline owning the flight number as well as by another airliner.</li> <li><b>1 - IsOperator</b>: Flight is operated by an airline owning the flight number (the same code)</li> <li><b>2 - IsCodeshared</b>: Flight is code-shared (operated by an airline other than airline owning the flight number)</li> </ul>'
layout: schema
name: CodeshareStatus
properties_list: []
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-codeshare-status-schema.json
slug: aerodatabox-codeshare-status
source_filename: aerodatabox-codeshare-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-codeshare-status-schema.json\",\n  \"title\": \"CodeshareStatus\",\n  \"description\": \"Flight code-share status<p>Possible values:</p>\\r\\n<ul>\\r\\n<li><b>0 - Unknown</b>: Code-sharing information is unavailable for this flight. Flight might be operated both by airline owning the flight number as well as by another airliner.</li>\\r\\n<li><b>1 - IsOperator</b>: Flight is operated by an airline owning the flight number (the same code)</li>\\r\\n<li><b>2 - IsCodeshared</b>: Flight is code-shared (operated by an airline other than airline owning the flight number)</li>\\r\\n</ul>\\r\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Unknown\",\n    \"IsOperator\",\n    \"IsCodeshared\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-codeshare-status-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: CodeshareStatus
---
