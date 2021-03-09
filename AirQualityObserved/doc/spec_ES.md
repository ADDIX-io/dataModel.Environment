Entidad: AirQualityObserved  
===========================  
[Licencia abierta](https://github.com/smart-data-models//dataModel.Environment/blob/master/AirQualityObserved/LICENSE.md)  
Descripción global: **Una observación de las condiciones de calidad del aire en un lugar y momento determinados.**  

## Lista de propiedades  

- `address`: La dirección postal.  - `airQualityIndex`: Índice de calidad del aire correspondiente a la calidad del aire observada  - `airQualityLevel`: Nivel cualitativo global de preocupación por la salud correspondiente a la calidad del aire observada  - `alternateName`: Un nombre alternativo para este artículo  - `areaServed`: Área de nivel superior a la que pertenece esta medición de la calidad del aire  - `as`: Arsénico detectado  - `c6h6`: Se ha detectado benceno  - `cd`: Cadmio detectado  - `co`: Monóxido de carbono detectado  - `dataProvider`: Una secuencia de caracteres que identifica al proveedor de la entidad de datos armonizada.  - `dateCreated`: Marca de tiempo de creación de la entidad. Suele ser asignada por la plataforma de almacenamiento.  - `dateModified`: Marca de tiempo de la última modificación de la entidad. Normalmente será asignada por la plataforma de almacenamiento.  - `dateObserved`: La fecha y la hora de esta observación en formato ISO8601 UTC  - `description`: Una descripción de este artículo  - `id`: Identificador único de la entidad  - `location`:   - `name`: El nombre de este artículo.  - `ni`: Níquel detectado  - `False`: Monóxido de nitrógeno detectado  - `no2`: Dióxido de nitrógeno detectado  - `o3`: Ozono detectado  - `owner`: Una lista que contiene una secuencia de caracteres codificada en JSON que hace referencia a los identificadores únicos de los propietarios  - `pb`: Plomo detectado  - `pm10`: Partículas de 10 micrómetros o menos de diámetro  - `pm25`: Partículas de 2,5 micrómetros o menos de diámetro  - `refDevice`: Una referencia al dispositivo o dispositivos que captaron esta observación.  - `refPointOfInterest`: Una referencia a un punto de interés (normalmente una estación de calidad del aire) asociada a esta observación.  - `refWeatherObserved`:  Tiempo observado asociado a las condiciones de calidad del aire descritas por esta entidad.  - `reliability`: Fiabilidad (porcentaje, expresado en partes por uno) correspondiente a la calidad del aire observada  - `seeAlso`: lista de uri que apuntan a recursos adicionales sobre el artículo  - `sh2`: Sulfuro de hidrógeno detectado  - `so2`: Dióxido de azufre detectado  - `source`: Una secuencia de caracteres que indica la fuente original de los datos de la entidad en forma de URL. Se recomienda que sea el nombre de dominio completo del proveedor de origen, o la URL del objeto de origen.  - `type`: NGSI Tipo de entidad  - `volatileOrganicCompoundsTotal`: Alcanos <C10, cetonas <C6, aldehídos <C10, ácidos carboxílicos <C5, aspirinas<C7, alquenos <C8, aromáticos    
Propiedades requeridas  
- `dateObserved`  - `id`  - `location`  - `type`  ## Descripción del modelo de datos de las propiedades  
Ordenados alfabéticamente (haga clic para ver los detalles)  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
AirQualityObserved:    
  description: 'An observation of air quality conditions at a certain place and time.'    
  properties:    
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
        areaServed:    
          description: 'Property. The geographic area where a service or offered item is provided. Model:''https://schema.org/areaServed'''    
          type: string    
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, Spain. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, Spain. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
      type: Property    
      x-ngsi:    
        model: https://schema.org/address    
    airQualityIndex:    
      description: 'Air quality index is a number used to report the quality of the air on any given day.'    
      minimum: 0    
      type: Property    
      x-ngsi:    
        model: https://schema.org/Number    
    airQualityLevel:    
      description: 'Overall qualitative level of health concern corresponding to the air quality observed'    
      minLength: 2    
      type: Property    
      x-ngsi:    
        model: 'https://schema.org/Tex '    
    alternateName:    
      description: 'An alternative name for this item'    
      type: Property    
    areaServed:    
      description: 'Higher level area to which this air quality measurement belongs to'    
      type: Property    
      x-ngsi:    
        model: 'https://schema.org/Text '    
    as:    
      description: 'Arsenic detected'    
      minimum: 0    
      type: Property    
      x-ngsi:    
        model: https://schema.org/Number    
    c6h6:    
      description: 'Benzene detected'    
      minimum: 0    
      type: Property    
    cd:    
      description: 'Cadmium detected'    
      minimum: 0    
      type: Property    
    co:    
      description: 'Carbon Monoxide detected'    
      minimum: 0    
      type: Property    
    co2:    
      description: 'Carbon Dioxide detected'    
      minimum: 0    
      type: Property    
    coLevel:    
      description: 'Qualitative Carbon Monoxide presence'    
      type: Property    
    dataProvider:    
      description: 'A sequence of characters identifying the provider of the harmonised data entity.'    
      type: Property    
    dateCreated:    
      description: 'Entity creation timestamp. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: Property    
    dateModified:    
      description: 'Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: Property    
    dateObserved:    
      description: 'The date and time of this observation in ISO8601 UTCformat'    
      type: Property    
      x-ngsi:    
        model: 'https://schema.org/Text '    
    description:    
      description: 'A description of this item'    
      type: Property    
    id:    
      anyOf: &airqualityobserved_-_properties_-_owner_-_items_-_anyof    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'Unique identifier of the entity'    
      type: Property    
    location:    
      $id: https://geojson.org/schema/Geometry.json    
      $schema: "http://json-schema.org/draft-07/schema#"    
      oneOf:    
        - properties:    
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
        - properties:    
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
        - properties:    
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
        - properties:    
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
        - properties:    
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
        - properties:    
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
      title: 'GeoJSON Geometry'    
    name:    
      description: 'The name of this item.'    
      type: Property    
    ni:    
      description: 'Nickel detected'    
      minimum: 0    
      type: Property    
    no:    
      description: 'Nitrogen monoxide detected'    
      minimum: 0    
      type: Property    
    no2:    
      description: 'Nitrogen dioxide detected'    
      minimum: 0    
      type: Property    
    nox:    
      description: 'Other Nitrogen oxides detected'    
      minimum: 0    
      type: Property    
    o3:    
      description: 'Ozone detected'    
      minimum: 0    
      type: Property    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf: *airqualityobserved_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: Property    
    pb:    
      description: 'Lead detected'    
      minimum: 0    
      type: Property    
    pm10:    
      description: 'Particulate matter 10 micrometers or less in diameter'    
      minimum: 0    
      type: Property    
    pm25:    
      description: 'Particulate matter 2.5 micrometers or less in diameter'    
      minimum: 0    
      type: Property    
    precipitation:    
      description: 'Amount of water rain'    
      minimum: 0    
      type: Property    
      x-ngsi:    
        model: https://schema.org/Number    
        units: 'Liters per square meter.'    
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
      description: 'A reference to the device(s) which captured this observation.'    
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
      description: 'A reference to a point of interest (usually an air quality station) associated to this observation.'    
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
      description: ' Weather observed associated to the air quality conditions described by this entity.'    
      type: Relationship    
    relativeHumidity:    
      description: 'Humidity in the Air'    
      maximum: 1    
      minimum: 0    
      type: Property    
      x-ngsi:    
        model: https://schema.org/Number    
    reliability:    
      description: 'Reliability (percentage, expressed in parts per one) corresponding to the air quality observed'    
      maximum: 1.0    
      minimum: 0    
      type: Property    
      x-ngsi:    
        model: 'https://schema.org/Number '    
    seeAlso:    
      description: 'list of uri pointing to additional resources about the item'    
      oneOf:    
        - items:    
            - format: uri    
              type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      type: Property    
    sh2:    
      description: 'Hydrogen sulfide detected'    
      minimum: 0    
      type: Property    
    so2:    
      description: 'Sulfur dioxide detected'    
      minimum: 0    
      type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: Property    
    temperature:    
      description: 'Temperature of the item'    
      type: Property    
    type:    
      description: 'NGSI Entity type'    
      enum:    
        - AirQualityObserved    
      type: Property    
    typeofLocation:    
      description: 'Type of location of the sampled item'    
      enum:    
        - indoor    
        - outdoor    
      type: Property    
      x-ngsi:    
        model: https://schema.org/Text    
    volatileOrganicCompoundsTotal:    
      description: 'Alkanes <C10, ketones <C6, aldehydes <C10, carboxylic acids <C5, aspirits<C7, Alkenes <C8, Aromatics'    
      minimum: 0    
      type: Property    
    windDirection:    
      description: 'Direction of the weather vane'    
      maximum: 180    
      minimum: -180    
      type: Property    
      x-ngsi:    
        model: http://schema.org/Number    
    windSpeed:    
      description: 'Intensity of the wind'    
      minimum: 0    
      type: Property    
      x-ngsi:    
        model: http//schema.org/Number    
  required:    
    - id    
    - type    
    - dateObserved    
    - location    
  type: object    
```  
</details>    
## Ejemplo de carga útil  
#### AirQualityObserved NGSI V2 key-values Ejemplo  
Aquí hay un ejemplo de un AirQualityObserved en formato JSON como key-values. Esto es compatible con NGSI V2 cuando se utiliza `options=keyValues` y devuelve los datos de contexto de una entidad individual.  
```json  
{  
  "id": "Madrid-AmbientObserved-28079004-2016-03-15T11:00:00",  
  "type": "AirQualityObserved",  
  "address": {  
    "addressCountry": "ES",  
    "addressLocality": "Madrid",  
    "streetAddress": "Plaza de España"  
  },  
  "dateObserved": "2016-03-15T11:00:00/2016-03-15T12:00:00",  
  "areaServed": "Brooklands",  
  "location": {  
    "type": "Point",  
    "coordinates": [-3.712247222222222, 40.423852777777775]  
  },  
  "source": "http://datos.madrid.es",  
  "typeOfLocation": "outdoor",  
  "precipitation": 0,  
  "relativeHumidity": 0.54,  
  "temperature": 12.2,  
  "windDirection": 186,  
  "windSpeed": 0.64,  
  "airQualityLevel": "moderate",  
  "airQualityIndex": 65,  
  "reliability": 0.7,  
  "co": 500,  
  "no": 45,  
  "co2": 69,  
  "nox": 139,  
  "so2": 11,  
  "coLevel": "moderate",  
  "refPointOfInterest": "28079004-Pza.deEspanya"  
}  
```  
#### AirQualityObserved NGSI V2 normalizado Ejemplo  
Aquí hay un ejemplo de un AirQualityObserved en formato JSON normalizado. Esto es compatible con NGSI V2 cuando no se utilizan opciones y devuelve los datos de contexto de una entidad individual.  
```json  
{  
  "id": "Madrid-AmbientObserved-28079004-2016-03-15T11:00:00",  
  "type": "AirQualityObserved",  
  "dateObserved": {  
    "value": "2016-03-15T11:00:00/2016-03-15T12:00:00"  
  },  
  "areaServed": {  
    "value": "Brooklands"  
  },  
  "airQualityLevel": {  
    "value": "moderate"  
  },  
  "CO": {  
    "value": 500,  
    "metadata": {  
      "unitCode": {  
        "value": "GP"  
      }  
    }  
  },  
  "temperature": {  
    "value": 12.2  
  },  
  "NO": {  
    "value": 45,  
    "metadata": {  
      "unitCode": {  
        "value": "GQ"  
      }  
    }  
  },  
  "refPointOfInterest": {  
    "type": "Relationship",  
    "value": "28079004-Pza.deEspanya"  
  },  
  "windDirection": {  
    "value": 186  
  },  
  "source": {  
    "value": "http://datos.madrid.es"  
  },  
  "windSpeed": {  
    "value": 0.64  
  },  
  "SO2": {  
    "value": 11,  
    "metadata": {  
      "unitCode": {  
        "value": "GQ"  
      }  
    }  
  },  
  "NOx": {  
    "value": 139,  
    "metadata": {  
      "unitCode": {  
        "value": "GQ"  
      }  
    }  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [-3.712247222222222, 40.423852777777775]  
    }  
  },  
  "typeOfLocation": {  
    "value": "outdoor"  
  },  
  "airQualityIndex": {  
    "value": 65  
  },  
  "address": {  
    "type": "PostalAddress",  
    "value": {  
      "addressCountry": "ES",  
      "addressLocality": "Madrid",  
      "streetAddress": "Plaza de Espa\u00f1a"  
    }  
  },  
  "reliability": {  
    "value": 0.7  
  },  
  "relativeHumidity": {  
    "value": 0.54  
  },  
  "precipitation": {  
    "value": 0  
  },  
  "NO2": {  
    "value": 69,  
    "metadata": {  
      "unitCode": {  
        "value": "GQ"  
      }  
    }  
  },  
  "CO_Level": {  
    "value": "moderate"  
  }  
}  
```  
#### AirQualityObserved NGSI-LD key-values Ejemplo  
Aquí hay un ejemplo de un AirQualityObserved en formato JSON-LD como valores-clave. Esto es compatible con NGSI-LD cuando se utiliza `options=keyValues` y devuelve los datos de contexto de una entidad individual.  
```json  
{"@context": ["https://schema.lab.fiware.org/ld/context",  
              "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"],  
 "CO": 500,  
 "CO_Level": "moderate",  
 "NO": 45,  
 "NO2": 69,  
 "NOx": 139,  
 "SO2": 11,  
 "address": {"addressCountry": "ES",  
             "addressLocality": "Madrid",  
             "streetAddress": "Plaza de EspaÃ±a",  
             "type": "PostalAddress"},  
 "airQualityIndex": 65,  
 "airQualityLevel": "moderate",  
 "areaServed": "Brooklands",  
 "dateObserved": "2016-03-15T11:00:00/2016-03-15T12:00:00",  
 "id": "urn:ngsi-ld:AirQualityObserved:Madrid-AmbientObserved-28079004-2016-03-15T11:00:00",  
 "location": {"coordinates": [-3.712247222222222, 40.423852777777775],  
              "type": "Point"},  
 "typeOfLocation": "outdoor",  
 "precipitation": 0,  
 "refPointOfInterest": "urn:ngsi-ld:PointOfInterest:28079004-Pza.deEspanya",  
 "relativeHumidity": 0.54,  
 "reliability": 0.7,  
 "source": "http://datos.madrid.es",  
 "temperature": 12.2,  
 "type": "AirQualityObserved",  
 "windDirection": 186,  
 "windSpeed": 0.64}  
```  
#### AirQualityObserved NGSI-LD normalizado Ejemplo  
Este es un ejemplo de AirQualityObserved en formato JSON-LD normalizado. Esto es compatible con NGSI-LD cuando no se utilizan opciones y devuelve los datos de contexto de una entidad individual.  
```json  
{  
    "id": "urn:ngsi-ld:AirQualityObserved:Madrid-AmbientObserved-28079004-2016-03-15T11:00:00",  
    "type": "AirQualityObserved",  
    "dateObserved": {  
        "type": "Property",  
        "value": "2016-03-15T11:00:00/2016-03-15T12:00:00"  
    },  
    "areaServed": {  
        "type": "Property",  
        "value": "Brooklands"  
    },  
    "airQualityLevel": {  
        "type": "Property",  
        "value": "moderate"  
    },  
    "CO": {  
        "type": "Property",  
        "value": 500,  
        "unitCode": "GP"  
    },  
    "temperature": {  
        "type": "Property",  
        "value": 12.2  
    },  
    "NO": {  
        "type": "Property",  
        "value": 45,  
        "unitCode": "GQ"  
    },  
    "refPointOfInterest": {  
        "type": "Relationship",  
        "object": "urn:ngsi-ld:PointOfInterest:28079004-Pza.deEspanya"  
    },  
    "windDirection": {  
        "type": "Property",  
        "value": 186  
    },  
    "source": {  
        "type": "Property",  
        "value": "http://datos.madrid.es"  
    },  
    "windSpeed": {  
        "type": "Property",  
        "value": 0.64  
    },  
    "SO2": {  
        "type": "Property",  
        "value": 11,  
        "unitCode": "GQ"  
    },  
    "NOx": {  
        "type": "Property",  
        "value": 139,  
        "unitCode": "GQ"  
    },  
    "location": {  
        "type": "GeoProperty",  
        "value": {  
            "type": "Point",  
            "coordinates": [  
                -3.712247222222222,  
                40.423852777777775  
            ]  
        }  
    },  
    "typeOfLocation": {  
        "type": "Property",  
        "value": "outdoor"  
    },  
    "airQualityIndex": {  
        "type": "Property",  
        "value": 65  
    },  
    "address": {  
        "type": "Property",  
        "value": {  
            "addressCountry": "ES",  
            "addressLocality": "Madrid",  
            "streetAddress": "Plaza de EspaÃ±a",  
            "type": "PostalAddress"  
        }  
    },  
    "reliability": {  
        "type": "Property",  
        "value": 0.7  
    },  
    "relativeHumidity": {  
        "type": "Property",  
        "value": 0.54  
    },  
    "precipitation": {  
        "type": "Property",  
        "value": 0  
    },  
    "NO2": {  
        "type": "Property",  
        "value": 69,  
        "unitCode": "GQ"  
    },  
    "CO_Level": {  
        "type": "Property",  
        "value": "moderate"  
    },  
    "@context": [  
        "https://schema.lab.fiware.org/ld/context",  
        "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"  
    ]  
}  
```  
