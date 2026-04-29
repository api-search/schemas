---
description: 'Flight progress status<p>Possible values:</p> <ul> <li><b>0 - Unknown</b>: Status is not available for this flight</li> <li><b>1 - Expected</b>: Expected</li> <li><b>2 - EnRoute</b>: En route</li> <li><b>3 - CheckIn</b>: Check-in is open</li> <li><b>4 - Boarding</b>: Boarding in progress / Last call</li> <li><b>5 - GateClosed</b>: Gate closed</li> <li><b>6 - Departed</b>: Departed</li> <li><b>7 - Delayed</b>: Delayed</li> <li><b>8 - Approaching</b>: On approach to destination</li> <li><b>9 - Arrived</b>: Arrived</li> <li><b>10 - Canceled</b>: Cancelled</li> <li><b>11 - Diverted</b>: Diverted to another destination</li> <li><b>12 - CanceledUncertain</b>: Status of the flight is uncertain, may be cancelled</li> </ul>'
layout: schema
name: FlightStatus
properties_list: []
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-status-schema.json
slug: aerodatabox-flight-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-status-schema.json\",\n  \"title\": \"FlightStatus\",\n  \"description\": \"Flight progress status<p>Possible values:</p>\\r\\n<ul>\\r\\n<li><b>0 - Unknown</b>: Status is not available for this flight</li>\\r\\n<li><b>1 - Expected</b>: Expected</li>\\r\\n<li><b>2 - EnRoute</b>: En route</li>\\r\\n<li><b>3 - CheckIn</b>: Check-in is open</li>\\r\\n<li><b>4 - Boarding</b>: Boarding in progress / Last call</li>\\r\\n<li><b>5 - GateClosed</b>: Gate closed</li>\\r\\n<li><b>6 - Departed</b>: Departed</li>\\r\\n<li><b>7 - Delayed</b>: Delayed</li>\\r\\n<li><b>8 - Approaching</b>: On approach to destination</li>\\r\\n<li><b>9 - Arrived</b>: Arrived</li>\\r\\n<li><b>10 - Canceled</b>: Cancelled</li>\\r\\n<li><b>11 - Diverted</b>: Diverted to another destination</li>\\r\\n<li><b>12 - CanceledUncertain</b>:\
  \ Status of the flight is uncertain, may be cancelled</li>\\r\\n</ul>\\r\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Unknown\",\n    \"Expected\",\n    \"EnRoute\",\n    \"CheckIn\",\n    \"Boarding\",\n    \"GateClosed\",\n    \"Departed\",\n    \"Delayed\",\n    \"Approaching\",\n    \"Arrived\",\n    \"Canceled\",\n    \"Diverted\",\n    \"CanceledUncertain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-status-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightStatus
---
