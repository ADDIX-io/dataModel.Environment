<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entité : WaterObserved  
======================<!-- /10-Header -->  
<!-- 15-License -->  
[Licence ouverte] (https://github.com/smart-data-models//dataModel.Environment/blob/master/WaterObserved/LICENSE.md)  
[document généré automatiquement] (https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
Description globale : ** Le modèle de données d'observation de l'eau est destiné à représenter les paramètres de débit, de niveau et de volume d'eau observés, ainsi que les informations sur la houle, sur une zone fixe ou variable. Cette observation inclut également les masses d'objets flottants sur cette zone. Les données collectées sont fournies par des capteurs, des caméras, des stations d'observation de l'eau positionnées à des endroits spécifiques ou sensibles pour les rivières, les ruisseaux, les torrents, les lacs, les mers, etc.**.  
version : 0.0.2  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## Liste des propriétés  

<sup><sub>[*] S'il n'y a pas de type dans un attribut, c'est parce qu'il pourrait avoir plusieurs types ou différents formats/modèles</sub></sup>.  
- `address[object]`: L'adresse postale  . Model: [https://schema.org/address](https://schema.org/address)- `alternateName[string]`: Un nom alternatif pour cet élément  - `areaServed[string]`: La zone géographique où un service ou un article offert est fourni  . Model: [https://schema.org/Text](https://schema.org/Text)- `dataProvider[string]`: Une séquence de caractères identifiant le fournisseur de l'entité de données harmonisées.  - `dateCreated[string]`: Horodatage de la création de l'entité. Celui-ci sera généralement attribué par la plateforme de stockage.  - `dateModified[string]`: Horodatage de la dernière modification de l'entité. Il sera généralement attribué par la plateforme de stockage.  - `dateObserved[string]`: Date et heure de cette observation représentées par un format ISO8601 UTC.  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `dateObservedFrom[string]`: Période d'observation : Date et heure de début dans un format ISO8601 UTC.  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `dateObservedTo[string]`: Période d'observation : Date et heure de fin dans un format ISO8601 UTC.  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `description[string]`: Une description de cet article  - `flow[number]`: Débit d'eau observé. Le code d'unité (texte) de mesure donné à l'aide de la norme UN/CEFACAT  . Model: [https://schema.org/Number](https://schema.org/Number)- `height[number]`: Hauteur d'eau - Niveau atteint sur les côtes d'alerte.  . Model: [https://schema.org/height](https://schema.org/height)- `id[*]`: Identifiant unique de l'entité  - `location[*]`: Référence Geojson à l'élément. Il peut s'agir d'un point, d'une ligne, d'un polygone, d'un point multiple, d'une ligne multiple ou d'un polygone multiple.  - `measuredArea[number]`: Référence de la surface mesurée. Le code d'unité (texte) de mesure donné en utilisant les [Codes communs du CEFACT-ONU] (http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (3 caractères maximum). Par exemple, <code>MTK</code> représente M².  . Model: [https://schema.org/Number](https://schema.org/Number)- `name[string]`: Le nom de cet élément.  - `objectArea[number]`: Pourcentage occupé par un objet flottant dans la zone. Le code d'unité (texte) de mesure donné en utilisant les [Codes communs du CEFACT-ONU] (http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (3 caractères maximum). Par exemple, <code>P1</code> représente le Pourcentage.  . Model: [https://schema.org/Number](https://schema.org/Number)- `objectHeightAverage[number]`: Hauteur moyenne levée. Le code d'unité (texte) de mesure donné en utilisant les [Codes communs du CEFACT-ONU] (http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (3 caractères maximum). Par exemple, <code>MTR</code> représente le mètre.  . Model: [https://schema.org/Number](https://schema.org/Number)- `objectHeightMax[number]`: Hauteur maximale levée. Le code d'unité (texte) de mesure donné en utilisant les [Codes communs du CEFACT-ONU] (http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (3 caractères maximum). Par exemple, <code>MTR</code> représente le mètre.  . Model: [https://schema.org/Number](https://schema.org/Number)- `objectVolume[number]`: Estimation du volume levé. Le code d'unité (texte) de mesure donné en utilisant les [Codes communs du CEFACT-ONU] (http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (3 caractères maximum). Par exemple, <code>MTQ</code> représente les mètres cubes.  . Model: [https://schema.org/Number](https://schema.org/Number)- `owner[array]`: Une liste contenant une séquence de caractères codée en JSON référençant les identifiants uniques du ou des propriétaires.  - `refDevice[*]`: Une référence à un point d'intérêt associé à cette observation.  - `seeAlso[*]`: liste d'uri pointant vers des ressources supplémentaires sur l'article  - `source[string]`: Une séquence de caractères donnant la source originale des données de l'entité sous forme d'URL. Il est recommandé d'utiliser le nom de domaine entièrement qualifié du fournisseur source ou l'URL de l'objet source.  - `swellDirection[number]`: Direction des houles observées.  . Model: [https://schema.org/Number](https://schema.org/Number)- `swellHeight[number]`: Hauteur de la houle observée.  . Model: [https://schema.org/height](https://schema.org/height)- `swellPeriod[number]`: Période de houle observée.  . Model: [https://schema.org/Number](https://schema.org/Number)- `type[string]`: Type d'entité NGSI. Il doit s'agir de WaterObserved  - `waveLength[number]`: Longueur d'onde observée.  . Model: [https://schema.org/Number](https://schema.org/Number)<!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
Propriétés requises  
- `dateObserved`  - `id`  - `location`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
Le modèle de données d'observation de l'eau est destiné à représenter les paramètres de débit, de niveau et de volume d'eau observés, ainsi que les informations sur la houle, sur une zone fixe ou variable. Cette observation inclut également les masses d'objets flottants sur cette zone.  Les données collectées sont fournies par des [Capteurs], [Caméras], [Stations d'eau] positionnés à des endroits spécifiques ou sensibles pour les rivières, fleuves, torrents, lacs, mers, etc.  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## Description des propriétés du modèle de données  
Classés par ordre alphabétique (cliquez pour plus de détails)  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
WaterObserved:    
  description: ' Water observation data model is intended to represent the parameters of flow, level and volume of water observed, as well as the swell information, over a fixed or variable area. This observation also includes the masses of floating objects on this area. The data collected is provided by Sensors, Cameras,Water stations positioned at specific or sensitive locations for rivers, streams, torrent, lakes, seas, etc.'    
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
      description: 'Date and time of this observation represented by an ISO8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
    dateObservedFrom:    
      description: 'Observation period : Start date and time in an ISO8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
    dateObservedTo:    
      description: 'Observation period : End date and time in an ISO8601 UTC format.'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
    description:    
      description: 'A description of this item'    
      type: string    
      x-ngsi:    
        type: Property    
    flow:    
      description: 'Water Flow observed. The unit code (text) of measurement given using the UN/CEFACAT'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    height:    
      description: 'Water height - Level reach on alert coasts.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/height    
        type: Property    
    id:    
      anyOf: &waterobserved_-_properties_-_owner_-_items_-_anyof    
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
    measuredArea:    
      description: 'Reference of the surface measured. The unit code (text) of measurement given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (max. 3 characters). For instance, <code>MTK</code> represents M².'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: 'square meters'    
    name:    
      description: 'The name of this item.'    
      type: string    
      x-ngsi:    
        type: Property    
    objectArea:    
      description: 'Percentage occupied by floating object in the area. The unit code (text) of measurement given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (max. 3 characters). For instance, <code>P1</code> represents Percentage.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    objectHeightAverage:    
      description: 'Average height raised. The unit code (text) of measurement given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (max. 3 characters). For instance, <code>MTR</code> represents Meter.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: meters    
    objectHeightMax:    
      description: 'Maximum height raised. The unit code (text) of measurement given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (max. 3 characters). For instance, <code>MTR</code> represents Meter.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: meters    
    objectVolume:    
      description: 'Estimated volume raised. The unit code (text) of measurement given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes) (max. 3 characters). For instance, <code>MTQ</code> represents Cubic Meters'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
        units: 'cubic meters'    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf: *waterobserved_-_properties_-_owner_-_items_-_anyof    
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
      description: 'A reference to a point of interest associated to this observation.'    
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
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    swellDirection:    
      description: 'Swells Direction observed.'    
      maximum: 360    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    swellHeight:    
      description: 'Swell height observed.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/height    
        type: Property    
    swellPeriod:    
      description: 'Swells period observed.'    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
    type:    
      description: 'NGSI Entity type. It has to be WaterObserved'    
      enum:    
        - WaterObserved    
      type: string    
      x-ngsi:    
        type: Property    
    waveLength:    
      description: 'Wave Length observed. '    
      minimum: 0    
      type: number    
      x-ngsi:    
        model: https://schema.org/Number    
        type: Property    
  required:    
    - id    
    - type    
    - location    
    - dateObserved    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2021 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Environment/blob/master/WaterObserved/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/data-models/Environment/WaterObserved/schema.js    
  x-model-tags: ""    
  x-version: 0.0.2    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## Exemples de charges utiles  
#### Valeurs clés de la NGSI-v2 WaterObserved Exemple  
Voici un exemple d'un WaterObserved au format JSON-LD sous forme de valeurs-clés. Ceci est compatible avec la NGSI-v2 lorsqu'on utilise `options=keyValues` et renvoie les données contextuelles d'une entité individuelle.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "WaterObserved:MNCA-001",  
  "type": "WaterObserved",  
  "name": "STLRT-MNCA-AP-WO-012",  
  "alternateName": "Var River Alert for safety procedure for Airport",  
  "description": "Observation of Evolution of the water levels",  
  "location": {  
    "type": "Point",  
    "coordinates": [  
      43.664810,  
      7.196545  
    ]  
  },  
  "areaServed": "Nice Airport",  
  "refDevice": "Device:T2-NP-018",  
  "dateObserved": "2020-03-17T08:45:00.209Z",  
  "flow": 12,  
  "height": 3.52,  
  "measuredArea": 250,  
  "objectArea": 35,  
  "objectHeightAverage": 1.75,  
  "objectHeightMax": 2.25,  
  "objectVolume": 17.5,  
  "waterLevel": 2.4,  
  "waterDischarge": 3  
}  
```  
</details>  
#### EauObservée NGSI-v2 normalisée Exemple  
Voici un exemple d'un WaterObserved au format JSON-LD tel que normalisé. Ceci est compatible avec la NGSI-v2 lorsqu'elle n'utilise pas d'options et renvoie les données contextuelles d'une entité individuelle.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "WaterObserved:MNCA-001",  
  "type": "WaterObserved",  
  "name": {  
    "type": "Text",  
    "value": "STLRT-MNCA-AP-WO-012"  
  },  
  "alternateName": {  
    "type": "Text",  
    "value": "Var River Alert for safety procedure for Airport"  
  },  
  "description": {  
    "type": "Text",  
    "value": "Observation of Evolution of the water levels"  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        43.664810,  
        7.196545  
      ]  
    }  
  },  
  "areaServed": {  
    "type": "Text",  
    "value": "Nice Airport"  
  },  
  "refDevice": {  
    "type": "Relationship",  
    "value": "Device:T2-NP-018"  
  },  
  "dateObserved": {  
    "type": "DateTime",  
    "value": "2020-03-17T08:45:00.209Z"  
  },  
  "flow": {  
    "type": "Number",  
    "value": 12  
  },  
  "height": {  
    "type": "Number",  
    "value": 3.52  
  },  
  "measuredArea": {  
    "type": "Number",  
    "value": 250  
  },  
  "objectArea": {  
    "type": "Number",  
    "value": 35  
  },  
  "objectHeightAverage": {  
    "type": "Number",  
    "value": 1.75  
  },  
  "objectHeightMax": {  
    "type": "Number",  
    "value": 2.25  
  },  
  "objectVolume": {  
    "type": "Number",  
    "value": 17.5  
  },  
  "waterLevel": {  
    "type": "Number",  
    "value": 2.4  
  },  
  "waterDischarge": {  
    "type": "Number",  
    "value": 3  
  }  
}  
```  
</details>  
#### Valeurs-clés NGSI-LD de l'eau observée Exemple  
Voici un exemple d'un WaterObserved au format JSON-LD sous forme de valeurs-clés. Ceci est compatible avec NGSI-LD en utilisant `options=keyValues` et retourne les données contextuelles d'une entité individuelle.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "uri:ngsi:WaterObserved:MNCA-001",  
    "type": "WaterObserved",  
    "alternateName": "Var River Alert for safety procedure for Airport",  
    "areaServed": "Nice Airport",  
    "dateObserved": "2020-03-17T08:45:00.209Z",  
    "description": "Observation of Evolution of the water levels",  
    "flow": 12,  
    "height": 3.52,  
    "location": {  
        "type": "Point",  
        "coordinates": [  
            43.66481,  
            7.196545  
        ]  
    },  
    "measuredArea": 250,  
    "name": "STLRT-MNCA-AP-WO-012",  
    "objectArea": 35,  
    "objectHeightAverage": 1.75,  
    "objectHeightMax": 2.25,  
    "objectVolume": 17.5,  
    "refDevice": "uri:ngsi:Device:T2-NP-018",  
    "@context": [  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Environment/master/context.jsonld"  
    ]  
}  
```  
</details>  
#### EauObservée NGSI-LD normalisée Exemple  
Voici un exemple d'un WaterObserved au format JSON-LD tel que normalisé. Ce format est compatible avec NGSI-LD lorsqu'il n'utilise pas d'options et renvoie les données contextuelles d'une entité individuelle.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
    "id": "urn:ngsi:WaterObserved:MNCA-001",  
    "type": "WaterObserved",  
    "alternateName": {  
        "type": "Property",  
        "value": "Var River Alert for safety procedure for Airport"  
    },  
    "areaServed": {  
        "type": "Property",  
        "value": "Nice Airport"  
    },  
    "dateObserved": {  
        "type": "Relationship",  
        "object": "2020-03-17T08:45:00.209Z"  
    },  
    "description": {  
        "type": "Property",  
        "value": "Observation of Evolution of the water levels"  
    },  
    "flow": {  
        "type": "Number",  
        "value": 12  
    },  
    "height": {  
        "type": "Number",  
        "value": 3.52  
    },  
    "location": {  
        "type": "GeoProperty",  
        "value": {  
            "type": "Point",  
            "coordinates": [  
                43.66481,  
                7.196545  
            ]  
        }  
    },  
    "measuredArea": {  
        "type": "Number",  
        "value": 250  
    },  
    "name": {  
        "type": "Property",  
        "value": "STLRT-MNCA-AP-WO-012"  
    },  
    "objectArea": {  
        "type": "Number",  
        "value": 35  
    },  
    "objectHeightAverage": {  
        "type": "Number",  
        "value": 1.75  
    },  
    "objectHeightMax": {  
        "type": "Number",  
        "value": 2.25  
    },  
    "objectVolume": {  
        "type": "Number",  
        "value": 17.5  
    },  
    "refDevice": {  
        "type": "Relationship",  
        "object": "uri:ngsi:Device:T2-NP-018"  
    },  
    "@context": [  
        "https://raw.githubusercontent.com/smart-data-models/dataModel.Environment/master/context.jsonld"  
    ]  
}  
```  
</details><!-- /80-Examples -->  
<!-- 90-FooterNotes -->  
<!-- /90-FooterNotes -->  
<!-- 95-Units -->  
Voir [FAQ 10](https://smartdatamodels.org/index.php/faqs/) pour obtenir une réponse sur la façon de traiter les unités de magnitude.  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
