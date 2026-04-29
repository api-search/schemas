---
description: Delay information about a batch of flights
layout: schema
name: FlightBatchDelayContract
properties_list:
- description: Total number of flights in the the batch (including cancelled)
  name: numTotal
  type: integer
- description: Total number of flights in the batch, which were used to to calculate the delay information (including cancelled). Should equal to or less than `NumTotal`. The closer the value of this property to the
  name: numQualifiedTotal
  type: integer
- description: Total amount of flights in the batch
  name: numCancelled
  type: integer
- description: 'Median delay of flights in the batch (format: [-]hh:mm:ss). Value can be negative (therefore, means early occurence).'
  name: medianDelay
  type: string
- description: Normalized value on scale from 0.0 to 5.0 which corresponds with current amount of delays and cancellations in a given batch of flights (the less - the better).
  name: delayIndex
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-flight-batch-delay-contract-schema.json
slug: aerodatabox-flight-batch-delay-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-batch-delay-contract-schema.json\",\n  \"title\": \"FlightBatchDelayContract\",\n  \"description\": \"Delay information about a batch of flights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"numTotal\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of flights in the the batch (including cancelled)\",\n      \"format\": \"int32\"\n    },\n    \"numQualifiedTotal\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of flights in the batch, which were used to to calculate the\\r\\ndelay information (including cancelled). Should equal to or less than `NumTotal`.\\r\\n\\r\\nThe closer the value of this property to the value of `NumTotal`, the higher the\\r\\nreliability of delay information\",\n      \"format\": \"int32\"\n    },\n    \"\
  numCancelled\": {\n      \"type\": \"integer\",\n      \"description\": \"Total amount of flights in the batch\",\n      \"format\": \"int32\"\n    },\n    \"medianDelay\": {\n      \"type\": \"string\",\n      \"description\": \"Median delay of flights in the batch (format: [-]hh:mm:ss).\\r\\nValue can be negative (therefore, means early occurence).\",\n      \"format\": \"date-span\",\n      \"nullable\": true\n    },\n    \"delayIndex\": {\n      \"type\": \"number\",\n      \"description\": \"Normalized value on scale from 0.0 to 5.0 which corresponds with current amount of delays and cancellations in a given batch of flights (the less - the better).\",\n      \"format\": \"float\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"numCancelled\",\n    \"numQualifiedTotal\",\n    \"numTotal\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-flight-batch-delay-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FlightBatchDelayContract
---
