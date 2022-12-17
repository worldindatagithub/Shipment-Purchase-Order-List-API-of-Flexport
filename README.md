# Working with the Shipment Purchase Order List API of Flexport #
The Flexport shipment purchase order list API allows developers to retrieve a list of purchase order line items or a specific line item. Its purpose is to provide an easy way to access and manage purchase orders within an application.

[Shipment Purchase Order List API](https://www.worldindata.com/api/Flexport-shipment-purchase-order-list-api)

Worldindata's data Marketplace is a resource that catalogues various APIs from third parties, with the goal of simplifying the process of understanding and utilizing these APIs. It offers a convenient way to discover and learn about new APIs that may be useful for your project.


## Clients, Industry, and Sectors ##

**Industry and Sectors**
- freight
- maritime
- logistics
- import
- export
- trade

**Client Types**
- freight and logistics companies
- importers
- exporters
- international traders




## API Parameters, JSON output and Objects ##
The GET /purchase_order_line_items endpoint allows developers to retrieve a list of purchase order line items or a specific line item using the Flexport shipment purchase orders API.

**filter parameters**
- page
- per
- direction
- f.purchase_order.id
- f.line_item_number
- f.item_key
- id


```
{
  "_object": "/api/response",
  "self": "https://api.flexport.com/purchase_orders?page=13&per=10",
  "version": 3,
  "data": {
    "_object": "/api/collections/paginated",
    "prev": "https://api.flexport.com/purchase_orders?page=12&per=10",
    "next": null,
    "data": [
      {
        "_object": "/purchase_orders/line_item",
        "id": 123456,
        "purchase_order": {
          "_object": "/api/refs/object",
          "ref_type": "/purchase_order",
          "link": "https://api.flexport.com/purchase_orders/26088",
          "id": 12345
        },
        "line_item_number": 1,
        "product": {
          "_object": "/purchase_order/line_item_product",
          "sku": "SKU-123",
          "name": "AC Adapter 12",
          "product_category": "furniture",
          "color": "red",
          "country_of_origin": "US",
          "dangerous": true,
          "ean_ucc_13": "1234567890123",
          "ean_ucc_8": "12345678",
          "lot_number": "123456789",
          "size": "m",
          "style": "classic",
          "upc": "123456789"
        },
        "assigned_party": {
          "_object": "/company_entity",
          "id": 9281,
          "name": "My Manufacturer",
          "ref": "manufacturer_1",
          "mailing_address": {
            "_object": "/address",
            "street_address": "1641 Settlers Lane",
            "street_address2": "STE 2918",
            "city": "Albany",
            "state": "MN",
            "country": "United States of America",
            "country_code": "US",
            "zip": "56307",
            "unlocode": "US AL2",
            "timezone": "America/Los_Angeles",
            "ref": null
          },
          "vat_numbers": [
            {
              "_object": "company_entity/vat_number",
              "country_code": "US",
              "number": "US 123746396"
            }
          ]
        },
        "item_key": "item1",
        "line_type": "main_line",
        "parent_line_key": null,
        "measurements": [
          {
            "_object": "/line_item_measure",
            "measure_type": "length",
            "unit_of_measure": "EA",
            "value": "1.0"
          }
        ],
        "units": 20,
        "incoterm": "FOB",
        "transportation_mode": "air",
        "unit_of_measure": "HUN",
        "must_arrive_date": "2019-03-11",
        "origin_port": null,
        "origin_location": {
          "_object": "/address",
          "street_address": "10th YouSong Industrial District",
          "street_address2": null,
          "city": "Shenzhen",
          "state": "44",
          "country": "China",
          "country_code": "CN",
          "timezone": "China/Shenzhen",
          "zip": null,
          "unlocode": null,
          "ref": "sellingcoaddress"
        },
        "destination_port": null,
        "metadata": {
          "size": [
            "M"
          ]
        },
        "destination_addresses": [
          {
            "address": {
              "_object": "/address",
              "street_address": "1556 20TH ST STE 2D",
              "street_address2": null,
              "city": "SANTA MONICA",
              "state": "CA",
              "country": "United States",
              "country_code": "US",
              "zip": "90404-3465",
              "unlocode": null,
              "ref": "studiosantamonica",
              "timezone": "America/Los Angeles"
            },
            "units": 1
          }
        ],
        "hs_codes": [
          {
            "_object": "/hs_code",
            "code": "8309.90.10.00",
            "country_code": "US"
          }
        ],
        "unit_cost": {
          "_object": "/money",
          "amount": "121.00",
          "currency_code": "USD"
        },
        "booking_line_items": {
          "_object": "/api/refs/collection",
          "ref_type": "/purchase_orders/booking_line_item",
          "link": "https://api.flexport.com/booking_line_items?f.purchase_order_line_item.id=123456"
        }
      }
    ]
  }
}

```
**Objects**
- purchase_order
- _object
- ref_type
- link
- id
- line_item_number
- product
- _object
- sku
- name
- product_category
- color
- country_of_origin
- dangerous
- ean_ucc_13
- ean_ucc_8
- lot_number
- size
- style
- upc

## Software Development Kit of the API ##
Software Development Kits (SDKs) for the Flexport shipment purchase orders API are available in a variety of programming languages including JAVA, PHP, Ruby, Python, and JavaScript. These SDKs make it easy for developers to integrate the API into their projects and take advantage of its features.

### Legal disclaimer ###
Worldindata is a resource that aims to make data in the world more user-friendly and help connect developers with data providers. While we do not own the data that is available through our platform, we are big fans of the Flexport shipment purchase order list API and are happy to provide a convenient way for developers to access and utilize this valuable resource. It is important to note that we are not affiliated with Flexport and this disclaimer is provided for legal purposes only.


[Worldindata](https://www.worldindata.com)
