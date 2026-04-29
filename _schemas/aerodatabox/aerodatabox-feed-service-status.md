---
description: 'Descriptor of feed service status<p>Possible values:</p> <ul> <li><b>0 - Down</b>: Service is provided, but is currently down</li> <li><b>1 - Degraded</b>: Service is up and running, but performance is degraded: delays and disruptions are likely</li> <li><b>2 - OKPartial</b>: Service is up and running normally, but updates vailable for not all or only few flights</li> <li><b>3 - OK</b>: Service is up and running normally</li> <li><b>-2 - Unknown</b>: Status of service is unknown</li> <li><b>-1 - Unavailable</b>: Service is not provided</li> </ul>'
layout: schema
name: FeedServiceStatus
properties_list: []
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-feed-service-status-schema.json
slug: aerodatabox-feed-service-status
source_filename: aerodatabox-feed-service-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-feed-service-status-schema.json\",\n  \"title\": \"FeedServiceStatus\",\n  \"description\": \"Descriptor of feed service status<p>Possible values:</p>\\r\\n<ul>\\r\\n<li><b>0 - Down</b>: Service is provided, but is currently down</li>\\r\\n<li><b>1 - Degraded</b>: Service is up and running, but performance is degraded: delays and disruptions are likely</li>\\r\\n<li><b>2 - OKPartial</b>: Service is up and running normally, but updates vailable for not all or only few flights</li>\\r\\n<li><b>3 - OK</b>: Service is up and running normally</li>\\r\\n<li><b>-2 - Unknown</b>: Status of service is unknown</li>\\r\\n<li><b>-1 - Unavailable</b>: Service is not provided</li>\\r\\n</ul>\\r\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Down\",\n    \"Degraded\",\n    \"OKPartial\",\n    \"OK\",\n\
  \    \"Unknown\",\n    \"Unavailable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-feed-service-status-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FeedServiceStatus
---
