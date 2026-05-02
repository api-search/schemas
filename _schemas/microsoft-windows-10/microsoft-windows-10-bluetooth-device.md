---
description: Schema for Windows 10 Bluetooth device data including Classic and Low Energy (BLE) devices as defined by the Windows.Devices.Bluetooth namespace. Covers BluetoothDevice, BluetoothLEDevice, GATT services and characteristics, RFCOMM services, and BLE advertisements.
layout: schema
name: Windows 10 Bluetooth Device
properties_list:
- description: Device identifier
  name: id
  type: string
- description: Device display name
  name: name
  type: string
- description: Bluetooth MAC address in XX:XX:XX:XX:XX:XX format
  name: bluetoothAddress
  type: string
- description: Bluetooth device type
  name: type
  type: string
- description: Current connection status (BluetoothConnectionStatus)
  name: connectionStatus
  type: string
- description: Whether the device is paired
  name: isPaired
  type: boolean
- description: ''
  name: classOfDevice
  type: object
- description: ''
  name: appearance
  type: object
- description: GATT services (for BLE devices)
  name: services
  type: array
- description: RFCOMM services (for Classic devices)
  name: rfcommServices
  type: array
provider_name: Microsoft Windows 10
provider_slug: microsoft-windows-10
schema_file: json-schema/microsoft-windows-10-bluetooth-device-schema.json
slug: microsoft-windows-10-bluetooth-device
source_filename: microsoft-windows-10-bluetooth-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.microsoft.com/schemas/windows-10/bluetooth-device.json\",\n  \"title\": \"Windows 10 Bluetooth Device\",\n  \"description\": \"Schema for Windows 10 Bluetooth device data including Classic and Low Energy (BLE) devices as defined by the Windows.Devices.Bluetooth namespace. Covers BluetoothDevice, BluetoothLEDevice, GATT services and characteristics, RFCOMM services, and BLE advertisements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Device identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device display name\"\n    },\n    \"bluetoothAddress\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\",\n      \"description\": \"Bluetooth MAC address in XX:XX:XX:XX:XX:XX format\"\n    },\n    \"type\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\"Classic\", \"LowEnergy\", \"Dual\"],\n      \"description\": \"Bluetooth device type\"\n    },\n    \"connectionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Connected\", \"Disconnected\"],\n      \"description\": \"Current connection status (BluetoothConnectionStatus)\"\n    },\n    \"isPaired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the device is paired\"\n    },\n    \"classOfDevice\": {\n      \"$ref\": \"#/$defs/ClassOfDevice\"\n    },\n    \"appearance\": {\n      \"$ref\": \"#/$defs/BluetoothLEAppearance\"\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/GattService\"\n      },\n      \"description\": \"GATT services (for BLE devices)\"\n    },\n    \"rfcommServices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RfcommService\"\n      },\n      \"description\": \"RFCOMM services (for Classic devices)\"\n    }\n  },\n  \"required\"\
  : [\"id\", \"name\", \"type\"],\n  \"$defs\": {\n    \"ClassOfDevice\": {\n      \"type\": \"object\",\n      \"description\": \"Bluetooth Class of Device (for Classic devices)\",\n      \"properties\": {\n        \"majorClass\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Miscellaneous\", \"Computer\", \"Phone\", \"NetworkAccessPoint\",\n            \"AudioVideo\", \"Peripheral\", \"Imaging\", \"Wearable\", \"Toy\",\n            \"Health\", \"Uncategorized\"\n          ],\n          \"description\": \"Major device class\"\n        },\n        \"minorClass\": {\n          \"type\": \"string\",\n          \"description\": \"Minor device class\"\n        },\n        \"serviceCapabilities\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"LimitedDiscoverableMode\", \"PositioningService\", \"NetworkingService\",\n              \"RenderingService\", \"CapturingService\", \"ObjectTransferService\"\
  ,\n              \"AudioService\", \"TelephonyService\", \"InformationService\"\n            ]\n          },\n          \"description\": \"Service capability flags\"\n        },\n        \"rawValue\": {\n          \"type\": \"integer\",\n          \"description\": \"Raw Class of Device value\"\n        }\n      }\n    },\n    \"BluetoothLEAppearance\": {\n      \"type\": \"object\",\n      \"description\": \"BLE device appearance (BluetoothLEAppearance class)\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"integer\",\n          \"description\": \"Appearance category value\"\n        },\n        \"subCategory\": {\n          \"type\": \"integer\",\n          \"description\": \"Appearance sub-category value\"\n        },\n        \"rawValue\": {\n          \"type\": \"integer\",\n          \"description\": \"Raw appearance value\"\n        }\n      }\n    },\n    \"GattService\": {\n      \"type\": \"object\",\n      \"description\": \"A GATT service on a BLE\
  \ device (GattDeviceService class)\",\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Service UUID\"\n        },\n        \"attributeHandle\": {\n          \"type\": \"integer\",\n          \"description\": \"GATT attribute handle\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Standard service name (if recognized)\"\n        },\n        \"characteristics\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/GattCharacteristic\"\n          }\n        },\n        \"parentServices\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"description\": \"UUIDs of parent services (for included services)\"\n        }\n      },\n      \"required\": [\"uuid\"]\n    },\n    \"GattCharacteristic\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"A GATT characteristic (GattCharacteristic class)\",\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Characteristic UUID\"\n        },\n        \"attributeHandle\": {\n          \"type\": \"integer\",\n          \"description\": \"GATT attribute handle\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Standard characteristic name (if recognized)\"\n        },\n        \"characteristicProperties\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"None\", \"Broadcast\", \"Read\", \"WriteWithoutResponse\", \"Write\",\n              \"Notify\", \"Indicate\", \"AuthenticatedSignedWrites\",\n              \"ExtendedProperties\", \"ReliableWrites\", \"WritableAuxiliaries\"\n            ]\n          },\n          \"description\": \"\
  Supported operations (GattCharacteristicProperties flags)\"\n        },\n        \"protectionLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"Plain\", \"AuthenticationRequired\", \"EncryptionRequired\", \"EncryptionAndAuthenticationRequired\"],\n          \"description\": \"Required protection level (GattProtectionLevel)\"\n        },\n        \"descriptors\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/GattDescriptor\"\n          }\n        },\n        \"userDescription\": {\n          \"type\": \"string\",\n          \"description\": \"User-friendly description from the Characteristic User Description descriptor\"\n        },\n        \"presentationFormats\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/GattPresentationFormat\"\n          }\n        }\n      },\n      \"required\": [\"uuid\", \"characteristicProperties\"]\n    },\n    \"GattDescriptor\": {\n      \"type\":\
  \ \"object\",\n      \"description\": \"A GATT descriptor (GattDescriptor class)\",\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"attributeHandle\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"required\": [\"uuid\"]\n    },\n    \"GattPresentationFormat\": {\n      \"type\": \"object\",\n      \"description\": \"Presentation format for a GATT characteristic\",\n      \"properties\": {\n        \"formatType\": {\n          \"type\": \"integer\",\n          \"description\": \"Format type byte\"\n        },\n        \"exponent\": {\n          \"type\": \"integer\"\n        },\n        \"unit\": {\n          \"type\": \"integer\",\n          \"description\": \"Unit UUID (16-bit)\"\n        },\n        \"namespace\": {\n          \"type\": \"integer\"\n        },\n        \"description\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"RfcommService\": {\n     \
  \ \"type\": \"object\",\n      \"description\": \"An RFCOMM service (RfcommDeviceService class)\",\n      \"properties\": {\n        \"serviceId\": {\n          \"type\": \"string\",\n          \"description\": \"RFCOMM service UUID\"\n        },\n        \"connectionHostName\": {\n          \"type\": \"string\"\n        },\n        \"connectionServiceName\": {\n          \"type\": \"string\"\n        },\n        \"maxProtocolDataUnit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum PDU size\"\n        }\n      },\n      \"required\": [\"serviceId\"]\n    },\n    \"BLEAdvertisement\": {\n      \"type\": \"object\",\n      \"description\": \"A BLE advertisement received by BluetoothLEAdvertisementWatcher\",\n      \"properties\": {\n        \"bluetoothAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Advertiser Bluetooth address\"\n        },\n        \"advertisementType\": {\n          \"type\": \"string\",\n          \"enum\": [\n\
  \            \"ConnectableUndirected\", \"ConnectableDirected\",\n            \"ScannableUndirected\", \"NonConnectableUndirected\", \"ScanResponse\"\n          ],\n          \"description\": \"Advertisement type\"\n        },\n        \"rawSignalStrengthInDBm\": {\n          \"type\": \"integer\",\n          \"description\": \"RSSI in dBm\"\n        },\n        \"localName\": {\n          \"type\": \"string\",\n          \"description\": \"Device local name from advertisement\"\n        },\n        \"serviceUuids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"description\": \"Advertised service UUIDs\"\n        },\n        \"manufacturerData\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"companyId\": {\n                \"type\": \"integer\"\n              },\n              \"data\"\
  : {\n                \"type\": \"string\",\n                \"format\": \"byte\"\n              }\n            }\n          },\n          \"description\": \"Manufacturer-specific data sections\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      },\n      \"required\": [\"bluetoothAddress\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/json-schema/microsoft-windows-10-bluetooth-device-schema.json
tags:
- Desktop
- Operating System
- UWP
- Win32
- Windows
title: Windows 10 Bluetooth Device
---
