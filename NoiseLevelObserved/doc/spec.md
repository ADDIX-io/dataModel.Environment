<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entity: NoiseLevelObserved  
==========================<!-- /10-Header -->  
<!-- 15-License -->  
[Open License](https://github.com/smart-data-models//dataModel.Environment/blob/master/NoiseLevelObserved/LICENSE.md)  
[document generated automatically](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
Global description: **An observation of those acoustic parameters that estimate noise pressure levels at a certain place and time. **  
version: 0.2.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## List of properties  

<sup><sub>[*] If there is not a type in an attribute is because it could have several types or different formats/patterns</sub></sup>  
- `LAS[number]`: The frequency weighted sound level (A-weighting) for a slow sound, one second mor more up and down.  - `LAeq[number]`: The frequency weighted Leq sound level (A-weighting).  - `LAeq_d[number]`: Acoustic Level frequency weigthed (A-weghting) equivalent for  a day  - `LAmax[number]`: Acoustic level frequency weigthed (A-weghting) maximum sound level  - `address[object]`: The mailing address  . Model: [https://schema.org/address](https://schema.org/address)- `alternateName[string]`: An alternative name for this item  - `areaServed[string]`: The geographic area where a service or offered item is provided  . Model: [https://schema.org/Text](https://schema.org/Text)- `dataProvider[string]`: A sequence of characters identifying the provider of the harmonised data entity.  - `dateCreated[string]`: Entity creation timestamp. This will usually be allocated by the storage platform.  - `dateModified[string]`: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.  - `dateObserved[string]`: The date and time of this observation represented by an ISO8601 interval.  - `dateObservedFrom[string]`: Observation period start date and time.  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `dateObservedTo[string]`: Observation period end date and time. See dateObserved.  . Model: [https://schema.org/Text](https://schema.org/Text)- `description[string]`: A description of this item  - `distanceAverage[string]`: Average distance between sensor and potential noise sources  - `heightAverage[string]`: Type of potential obstacles between the sensor and the noise source  - `id[*]`: Unique identifier of the entity  - `location[*]`: Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon  - `name[string]`: The name of this item.  - `obstacles[string]`: Type of potential obstacles between the sensor and the noise source.  - `owner[array]`: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)  - `refDevice[*]`: A reference to the device which captured this observation.  - `refPointOfInterest[*]`: A reference to a point of interest associated to this observation.  - `refWeatherObserved[*]`: Reference to the associated weather conditions.  - `seeAlso[*]`: list of uri pointing to additional resources about the item  - `sonometerClass[string]`: Class of sonometer (0, 1, 2) according to ANSI used for taking this observation  . Model: [https://schema.org/Text](https://schema.org/Text)- `source[string]`: A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.  - `type[string]`: NGSI Entity type  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
Required properties  
- `dateObservedFrom`  - `dateObservedTo`  - `id`  - `location`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## Data Model description of properties  
Sorted alphabetically (click for details)  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
NoiseLevelObserved:    
  description: 'An observation of those acoustic parameters that estimate noise pressure levels at a certain place and time. '    
  properties:    
    LAS:    
      description: 'The frequency weighted sound level (A-weighting) for a slow sound, one second mor more up and down.'    
      type: number    
      x-ngsi:    
        type: Property    
    LAeq:    
      description: 'The frequency weighted Leq sound level (A-weighting).'    
      type: number    
      x-ngsi:    
        type: Property    
    LAeq_d:    
      description: 'Acoustic Level frequency weigthed (A-weghting) equivalent for  a day'    
      type: number    
      x-ngsi:    
        type: Property    
    LAmax:    
      description: 'Acoustic level frequency weigthed (A-weghting) maximum sound level'    
      type: number    
      x-ngsi:    
        type: Property    
    address:    
      description: 'The mailing address'    
      properties:    
        addressCountry:    
          description: 'Property. The country. For example, Spain. Model:''https://schema.org/addressCountry'''    
          type: string    
        addressLocality:    
          description: 'Property. The locality in which the street address is, and which is in the region. Model:''https://schema.org/addressLocality'''    
          type: string    
        addressRegion:    
          description: 'Property. The region in which the locality is, and which is in the country. Model:''https://schema.org/addressRegion'''    
          type: string    
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, 03578. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, 24004. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    alternateName:    
      description: 'An alternative name for this item'    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: 'The geographic area where a service or offered item is provided'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    dataProvider:    
      description: 'A sequence of characters identifying the provider of the harmonised data entity.'    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: 'Entity creation timestamp. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: 'Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateObserved:    
      description: 'The date and time of this observation represented by an ISO8601 interval.'    
      type: string    
      x-ngsi:    
        type: Property    
    dateObservedFrom:    
      description: 'Observation period start date and time.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
    dateObservedTo:    
      description: 'Observation period end date and time. See dateObserved.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    description:    
      description: 'A description of this item'    
      type: string    
      x-ngsi:    
        type: Property    
    distanceAverage:    
      description: 'Average distance between sensor and potential noise sources'    
      type: string    
      x-ngsi:    
        type: Property    
        units: meters    
    heightAverage:    
      description: 'Type of potential obstacles between the sensor and the noise source'    
      type: string    
      x-ngsi:    
        type: Property    
        units: meters    
    id:    
      anyOf: &noiselevelobserved_-_properties_-_owner_-_items_-_anyof    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'Unique identifier of the entity'    
      x-ngsi:    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: 'GeoProperty. Geojson reference to the item. Point'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                type: number    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - Point    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON Point'    
          type: object    
        - description: 'GeoProperty. Geojson reference to the item. LineString'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - LineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON LineString'    
          type: object    
        - description: 'GeoProperty. Geojson reference to the item. Polygon'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 4    
                type: array    
              type: array    
            type:    
              enum:    
                - Polygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON Polygon'    
          type: object    
        - description: 'GeoProperty. Geojson reference to the item. MultiPoint'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPoint    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON MultiPoint'    
          type: object    
        - description: 'GeoProperty. Geojson reference to the item. MultiLineString'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiLineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON MultiLineString'    
          type: object    
        - description: 'GeoProperty. Geojson reference to the item. MultiLineString'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    items:    
                      type: number    
                    minItems: 2    
                    type: array    
                  minItems: 4    
                  type: array    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPolygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON MultiPolygon'    
          type: object    
      x-ngsi:    
        type: GeoProperty    
    name:    
      description: 'The name of this item.'    
      type: string    
      x-ngsi:    
        type: Property    
    obstacles:    
      description: 'Type of potential obstacles between the sensor and the noise source.'    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf: *noiselevelobserved_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Property    
    refDevice:    
      anyOf:    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'A reference to the device which captured this observation.'    
      x-ngsi:    
        type: Relationship    
    refPointOfInterest:    
      anyOf:    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'A reference to a point of interest associated to this observation.'    
      x-ngsi:    
        type: Relationship    
    refWeatherObserved:    
      anyOf:    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'Reference to the associated weather conditions.'    
      x-ngsi:    
        type: Relationship    
    seeAlso:    
      description: 'list of uri pointing to additional resources about the item'    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    sonometerClass:    
      description: 'Class of sonometer (0, 1, 2) according to ANSI used for taking this observation'    
      enum:    
        - 0    
        - 1    
        - 2    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    type:    
      description: 'NGSI Entity type'    
      enum:    
        - NoiseLevelObserved    
      type: string    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
    - dateObservedFrom    
    - dateObservedTo    
    - location    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2021 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Environment/blob/master/NoiseLevelObserved/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/dataModel.Environment/NoiseLevelObserved/schema.json    
  x-model-tags: GreenMov    
  x-version: 0.2.1    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## Example payloads    
#### NoiseLevelObserved NGSI-v2 key-values Example    
Here is an example of a NoiseLevelObserved in JSON-LD format as key-values. This is compatible with NGSI-v2 when  using `options=keyValues` and returns the context data of an individual entity.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "Vitoria-NoiseLevelObserved-2016-12-28T11:00:00_2016-12-28T12:00:00",  
  "type": "NoiseLevelObserved",  
  "LAS": 91.6,  
  "LAeq": 67.8,  
  "LAeq_d": 65.4,  
  "LAmax": 94.5,  
  "dateObservedFrom": "2016-12-28T11:00:00.00Z",  
  "dateObservedTo": "2016-12-28T12:00:00.00Z",  
  "location": {  
    "type": "Point",  
    "coordinates": [-2.698, 42.8491]  
  }  
}  
```  
</details>  
#### NoiseLevelObserved NGSI-v2 normalized Example    
Here is an example of a NoiseLevelObserved in JSON-LD format as normalized. This is compatible with NGSI-v2 when not using options and returns the context data of an individual entity.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "Vitoria-NoiseLevelObserved-2016-12-28T11:00:00_2016-12-28T12:00:00",  
  "type": "NoiseLevelObserved",  
  "dateObservedFrom": {  
    "type": "DateTime",  
    "value": "2016-12-28T11:00:00.00Z"  
  },  
  "LAmax": {  
    "type": "Number",  
    "value": 94.5  
  },  
  "LAeq": {  
    "type": "Number",  
    "value": 67.8  
  },  
  "dateObservedTo": {  
    "type": "DateTime",  
    "value": "2016-12-28T12:00:00.00Z"  
  },  
  "LAeq_d": {  
    "type": "Number",  
    "value": 65.4  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        -2.698,  
        42.8491  
      ]  
    }  
  },  
  "LAS": {  
    "type": "Number",  
    "value": 91.6  
  }  
}  
```  
</details>  
#### NoiseLevelObserved NGSI-LD key-values Example    
Here is an example of a NoiseLevelObserved in JSON-LD format as key-values. This is compatible with NGSI-LD when  using `options=keyValues` and returns the context data of an individual entity.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:ngsi-ld:NoiseLevelObserved:Vitoria-NoiseLevelObserved-2016-12-28T11:00:00_2016-12-28T12:00:00",  
    "type": "NoiseLevelObserved",  
    "LAS": 91.6,  
    "LAeq": 67.8,  
    "LAeq_d": 65.4,  
    "LAmax": 94.5,  
    "dateObservedFrom": {  
        "@type": "DateTime",  
        "@value": "2016-12-28T11:00:00.00Z"  
    },  
    "dateObservedTo": {  
        "@type": "DateTime",  
        "@value": "2016-12-28T12:00:00.00Z"  
    },  
    "location": {  
        "coordinates": [  
            -2.698,  
            42.8491  
        ],  
        "type": "Point"  
    },  
    "@context": [  
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Environment/master/context.jsonld"  
    ]  
}  
```  
</details>  
#### NoiseLevelObserved NGSI-LD normalized Example    
Here is an example of a NoiseLevelObserved in JSON-LD format as normalized. This is compatible with NGSI-LD when not using options and returns the context data of an individual entity.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:NoiseLevelObserved:Vitoria-NoiseLevelObserved-2016-12-28T11:00:00_2016-12-28T12:00:00",  
  "type": "NoiseLevelObserved",  
  "LAS": {  
    "type": "Property",  
    "value": 91.6  
  },  
  "LAeq": {  
    "type": "Property",  
    "value": 67.8  
  },  
  "LAeq_d": {  
    "type": "Property",  
    "value": 65.4  
  },  
  "LAmax": {  
    "type": "Property",  
    "value": 94.5  
  },  
  "dateObservedFrom": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2016-12-28T11:00:00.00Z"  
    }  
  },  
  "dateObservedTo": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2016-12-28T12:00:00.00Z"  
    }  
  },  
  "location": {  
    "type": "GeoProperty",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        -2.698,  
        42.8491  
      ]  
    }  
  },  
  "@context": [  
    "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.Environment/master/context.jsonld"  
  ]  
}  
```  
</details><!-- /80-Examples -->  
<!-- 90-FooterNotes -->  
<!-- /90-FooterNotes -->  
<!-- 95-Units -->  
See [FAQ 10](https://smartdatamodels.org/index.php/faqs/) to get an answer on how to deal with magnitude units  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
