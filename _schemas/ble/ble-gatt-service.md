---
description: Schema representing a Bluetooth GATT service definition as assigned by the Bluetooth SIG
layout: schema
name: BLE GATT Service
properties_list:
- description: 16-bit or 128-bit UUID assigned by Bluetooth SIG or custom
  name: uuid
  type: string
- description: Human-readable service name
  name: name
  type: string
- description: Whether this is a SIG-assigned or custom service
  name: type
  type: string
- description: GATT characteristics included in this service
  name: characteristics
  type: array
provider_name: BLE
provider_slug: ble
schema_file: json-schema/ble-gatt-service-schema.json
slug: ble-gatt-service
tags:
- BLE
- Bluetooth
- Embedded
- IoT
- Protocols
- Standards
- Wireless
title: BLE GATT Service
---
