---
description: Product information returned from a barcode lookup API query.
layout: schema
name: BarcodeLookupResponse
properties_list:
- description: The barcode number queried.
  name: barcode_number
  type: string
- description: The barcode format/symbology.
  name: barcode_type
  type: string
- description: URL of the barcode image.
  name: barcode_image
  type: string
- description: ''
  name: product
  type: object
provider_name: Barcode Scanners
provider_slug: barcode-scanners
schema_file: json-schema/barcode-lookup-schema.json
slug: barcode-lookup
tags:
- Barcodes
- Inventory
- Product Lookup
- QR Codes
- Retail
- Scanning
- Supply Chain
title: BarcodeLookupResponse
---
