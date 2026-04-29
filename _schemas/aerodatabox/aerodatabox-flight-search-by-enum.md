---
description: 'Criteria to search flight by<p>Possible values:</p> <ul> <li><b>0 - Number</b>: Search by flight number</li> <li><b>1 - Reg</b>: Search by aircraft registration</li> <li><b>2 - CallSign</b>: Search by ATC call-sign</li> <li><b>3 - Icao24</b>: Search by 24-bit ICAO Mode-S Transponder code</li> </ul>'
layout: schema
name: FlightSearchByEnum
properties_list: []
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-search-by-enum-schema.json
slug: aerodatabox-flight-search-by-enum
source_filename: aerodatabox-flight-search-by-enum-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-search-by-enum-schema.json\",\n  \"title\": \"FlightSearchByEnum\",\n  \"description\": \"Criteria to search flight by<p>Possible values:</p>\\r\\n<ul>\\r\\n<li><b>0 - Number</b>: Search by flight number</li>\\r\\n<li><b>1 - Reg</b>: Search by aircraft registration</li>\\r\\n<li><b>2 - CallSign</b>: Search by ATC call-sign</li>\\r\\n<li><b>3 - Icao24</b>: Search by 24-bit ICAO Mode-S Transponder code</li>\\r\\n</ul>\\r\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Number\",\n    \"Reg\",\n    \"CallSign\",\n    \"Icao24\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-search-by-enum-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightSearchByEnum
---
