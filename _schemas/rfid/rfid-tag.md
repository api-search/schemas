---
description: Schema representing an RFID tag read from a reader, including EPC, RSSI, and metadata
layout: schema
name: RFID Tag
properties_list:
- description: Electronic Product Code in hex or URN format
  name: epc
  type: string
- description: EPC in URN form per GS1 Tag Data Standard
  name: epcUrn
  type: string
- description: Tag Identifier memory bank (unique per chip)
  name: tidBank
  type: string
- description: Received Signal Strength Indicator in dBm
  name: rssi
  type: number
- description: Signal phase in degrees
  name: phase
  type: number
- description: Doppler shift frequency in Hz
  name: doppler
  type: number
- description: Antenna port ID on the reader that detected the tag
  name: antennaId
  type: integer
- description: Serial number of the RFID reader
  name: readerSerial
  type: string
- description: Hostname or IP of the RFID reader
  name: readerHostname
  type: string
- description: Time the tag was read
  name: timestamp
  type: string
- description: RFID tag air interface protocol
  name: tagType
  type: string
- description: Peak RSSI across multiple reads
  name: peakRssi
  type: number
- description: Number of times this tag was read in a session
  name: readCount
  type: integer
provider_name: RFID
provider_slug: rfid
schema_file: json-schema/rfid-tag-schema.json
slug: rfid-tag
source_filename: rfid-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/rfid/main/json-schema/rfid-tag-schema.json\",\n  \"title\": \"RFID Tag\",\n  \"description\": \"Schema representing an RFID tag read from a reader, including EPC, RSSI, and metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"epc\": {\n      \"type\": \"string\",\n      \"description\": \"Electronic Product Code in hex or URN format\",\n      \"example\": \"E280116060000204551400B5\"\n    },\n    \"epcUrn\": {\n      \"type\": \"string\",\n      \"description\": \"EPC in URN form per GS1 Tag Data Standard\",\n      \"example\": \"urn:epc:id:sgtin:0614141.107346.2017\"\n    },\n    \"tidBank\": {\n      \"type\": \"string\",\n      \"description\": \"Tag Identifier memory bank (unique per chip)\"\n    },\n    \"rssi\": {\n      \"type\": \"number\",\n      \"description\": \"Received Signal Strength Indicator in dBm\"\n    },\n    \"phase\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Signal phase in degrees\"\n    },\n    \"doppler\": {\n      \"type\": \"number\",\n      \"description\": \"Doppler shift frequency in Hz\"\n    },\n    \"antennaId\": {\n      \"type\": \"integer\",\n      \"description\": \"Antenna port ID on the reader that detected the tag\"\n    },\n    \"readerSerial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the RFID reader\"\n    },\n    \"readerHostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or IP of the RFID reader\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the tag was read\"\n    },\n    \"tagType\": {\n      \"type\": \"string\",\n      \"enum\": [\"UHF EPC Gen2\", \"HF ISO 15693\", \"HF ISO 14443A\", \"HF ISO 14443B\", \"LF 125kHz\", \"LF 134.2kHz\"],\n      \"description\": \"RFID tag air interface protocol\"\n    },\n    \"peakRssi\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Peak RSSI across multiple reads\"\n    },\n    \"readCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times this tag was read in a session\"\n    }\n  },\n  \"required\": [\"epc\", \"timestamp\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rfid/refs/heads/main/json-schema/rfid-tag-schema.json
tags:
- RFID
- IoT
- Supply Chain
- Inventory Management
- Asset Tracking
- GS1
- EPCIS
title: RFID Tag
---
