---
description: 'Criteria to search aircraft by<p>Possible values:</p> <ul> <li><b>0 - Id</b>: ID of the aircraft (as stored in this API)</li> <li><b>1 - Reg</b>: Search by aircraft tail-number</li> <li><b>2 - Icao24</b>: Search by 24-bit ICAO Mode-S Transponder code</li> </ul>'
layout: schema
name: AircraftSearchByEnum
properties_list: []
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-aircraft-search-by-enum-schema.json
slug: aerodatabox-aircraft-search-by-enum
source_filename: aerodatabox-aircraft-search-by-enum-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-search-by-enum-schema.json\",\n  \"title\": \"AircraftSearchByEnum\",\n  \"description\": \"Criteria to search aircraft by<p>Possible values:</p>\\r\\n<ul>\\r\\n<li><b>0 - Id</b>: ID of the aircraft (as stored in this API)</li>\\r\\n<li><b>1 - Reg</b>: Search by aircraft tail-number</li>\\r\\n<li><b>2 - Icao24</b>: Search by 24-bit ICAO Mode-S Transponder code</li>\\r\\n</ul>\\r\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Id\",\n    \"Reg\",\n    \"Icao24\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-aircraft-search-by-enum-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AircraftSearchByEnum
---
