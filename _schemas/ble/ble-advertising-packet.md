---
description: Schema for a decoded BLE advertising packet (ADV_IND or ADV_NONCONN_IND)
layout: schema
name: BLE Advertising Packet
properties_list:
- description: BLE device MAC address
  name: address
  type: string
- description: ''
  name: addressType
  type: string
- description: Received signal strength indicator in dBm
  name: rssi
  type: integer
- description: Complete or shortened local name
  name: localName
  type: string
- description: Advertised service UUIDs
  name: serviceUUIDs
  type: array
- description: ''
  name: manufacturerData
  type: object
- description: Transmit power level in dBm
  name: txPowerLevel
  type: integer
- description: Whether device accepts connections
  name: connectable
  type: boolean
provider_name: BLE
provider_slug: ble
schema_file: json-schema/ble-advertising-packet-schema.json
slug: ble-advertising-packet
tags:
- BLE
- Bluetooth
- Embedded
- IoT
- Protocols
- Standards
- Wireless
title: BLE Advertising Packet
---
