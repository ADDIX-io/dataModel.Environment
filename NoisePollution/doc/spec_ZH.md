<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
实体。噪声污染  
=======<!-- /10-Header -->  
<!-- 15-License -->  
[开放许可](https://github.com/smart-data-models//dataModel.Environment/blob/master/NoisePollution/LICENSE.md)  
[文件自动生成](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
全局描述。**噪声污染数据模型将具体和准时的噪声测量值（例如来自NoiseLevelObservation实体）合并为城市地区的平均参数，提供与城市有关的噪声污染状况和演变的更多数据**。  
版本：0.0.2  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

##属性列表  

<sup><sub>[*] 如果一个属性中没有一个类型，是因为它可能有几种类型或不同的格式/模式</sub></sup>。  
- `LAeq2[number]`: 过去2小时的平均声级  - `LAmax2[number]`: 过去2小时内记录的最大声级  - `alternateName[string]`: 这个项目的一个替代名称  - `buildingsType[string]`: 安装传感器时测量区域内主要建筑物的类型  - `dataProvider[string]`: 一串识别统一数据实体提供者的字符。  - `dateCreated[string]`: 实体创建时间戳。这通常会由存储平台分配。  - `dateModified[string]`: 实体最后一次修改的时间戳。这通常会由存储平台分配。  - `dateObservedFrom[string]`: 观察期开始日期和时间  - `dateObservedTo[string]`: 观察期的结束日期和时间  - `description[string]`: 对这个项目的描述  - `groundType[string]`: 安装传感器时测量区域的主要地面类型  - `id[*]`: 实体的唯一标识符  - `name[string]`: 这个项目的名称。  - `noiseAnnoyanceIndex[number]`: 根据噪音烦扰程度的指数（1至10）。  - `noiseOrigin[string]`: 传感器安装时记录的噪声的主要来源（源）。  - `owner[array]`: 一个包含JSON编码的字符序列的列表，引用所有者的唯一Ids。  - `seeAlso[*]`: 指向有关该项目的其他资源的URI列表  - `source[string]`: 一系列的字符，以URL的形式给出实体数据的原始来源。建议为源提供者的完全合格域名，或源对象的URL。  - `type[string]`: NGSI类型。它必须是NoisePollution  - `wallsType[string]`: 安装传感器时测量区域内的主要外墙材料类型  <!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
所需属性  
- `id`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## 数据模型的属性描述  
按字母顺序排列（点击查看详情）。  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
NoisePollution:    
  description: 'Noise Pollution data model merges specific and punctual noise measurements (coming, e.g. from NoiseLevelObservation entities) into average parameters referred to city areas, providing a more city-related data about noise pollution status and evolution.'    
  properties:    
    LAeq2:    
      description: 'Average sound level over the last 2 hours'    
      type: number    
      x-ngsi:    
        type: Property    
    LAmax2:    
      description: 'Maximum sound level recorded for the last 2 hours'    
      type: number    
      x-ngsi:    
        type: Property    
    alternateName:    
      description: 'An alternative name for this item'    
      type: string    
      x-ngsi:    
        type: Property    
    buildingsType:    
      description: 'Type of predominant buildings within the measurement area at installation of the sensor'    
      type: string    
      x-ngsi:    
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
    dateObservedFrom:    
      description: 'Observation period start date and time'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateObservedTo:    
      description: 'End date and time of the observation period'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: 'A description of this item'    
      type: string    
      x-ngsi:    
        type: Property    
    groundType:    
      description: 'Type of predominant ground in the measurement area at installation of the sensor'    
      type: string    
      x-ngsi:    
        type: Property    
    id:    
      anyOf: &noisepollution_-_properties_-_owner_-_items_-_anyof    
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
    name:    
      description: 'The name of this item.'    
      type: string    
      x-ngsi:    
        type: Property    
    noiseAnnoyanceIndex:    
      description: 'Index (1 to 10) according to noise annoyance level'    
      maximum: 10    
      minimum: 1    
      type: number    
      x-ngsi:    
        type: Property    
    noiseOrigin:    
      description: 'Main origin (source) of the recorded noise at installation of the sensor'    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf: *noisepollution_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Property    
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
    type:    
      description: 'NGSI type. it has to be NoisePollution'    
      enum:    
        - NoisePollution    
      type: string    
      x-ngsi:    
        type: Property    
    wallsType:    
      description: 'Facade material types dominant in the measurement area at installation of the sensor'    
      type: string    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2022 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Environment/blob/master/NoisePollution/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/dataModel.Environment/NoisePollution/schema.json    
  x-model-tags: ""    
  x-version: 0.0.2    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## ＃＃＃＃有效载荷的例子  
#### NoisePollution NGSI-v2 key-values 示例  
这里有一个以JSON-LD格式作为key-values的NoisePollution的例子。当使用`options=keyValues`时，这与NGSI-v2兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:NoisePollution:France-NoisePollution-12345_2022-07-01T18:00:00_2022-07-01T00:00:00",  
  "type": "NoisePollution",  
  "Laeq2": 85,  
  "Lamax2": 75,  
  "Lanight": 45,  
  "NoiseAnnoyanceIndex": 3,  
  "address": {  
    "addressCountry": "France",  
    "addressLocality": "Nice",  
    "postalCode": "06200",  
    "type": "PostalAddress"  
  },  
  "buildingsType": "residential",  
  "dataProvider": "IMREDD_UCA_Nice",  
  "dateObservedFrom": {  
    "@type": "DateTime",  
    "@value": "2022-07-01T10:40:01.00Z"  
  },  
  "dateObservedTo": {  
    "@type": "DateTime",  
    "@value": "2022-07-01T12:40:01.00Z"  
  },  
  "exposureType": "short term exposure",  
  "groundType": "concrete",  
  "location": {  
    "coordinates": [  
      7.2032497427380235,  
      43.68056738083439  
    ],  
    "type": "Point"  
  },  
  "noiseOrigin": "traffic",  
  "wallsType": "glass"  
}  
```  
</details>  
#### NoisePollution NGSI-v2归一化实例  
下面是一个以JSON-LD格式规范化的NoisePollution的例子。当不使用选项时，这与NGSI-v2兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:NoisePollution:France-NoisePollution-12345_2022-07-01T18:00:00_2022-07-01T00:00:00",  
  "type": "NoisePollution",  
  "address": {  
    "type": "StructuredValue",  
    "value": {  
      "addressCountry": "France",  
      "postalCode": "06200",  
      "addressLocality": "Nice",  
      "type": "PostalAddress"  
    }  
  },  
  "location": {  
    "type": "geo:json",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        7.2032497427380235,  
        43.68056738083439  
      ]  
    }  
  },  
  "dataProvider": {  
    "type": "Property",  
    "value": "IMREDD_UCA_Nice"  
  },  
  "dateObservedFrom": {  
    "type":  "DateTime",  
      "value": "2022-07-01T10:40:01.00Z"  
  },  
  "dateObservedTo": {  
    "type": "DateTime",  
      "value": "2022-07-01T12:40:01.00Z"  
  },  
  "NoiseAnnoyanceIndex": {  
    "type": "Number",  
    "value": 3  
  },  
  "Lanight": {  
    "type": "Number",  
    "value": 45  
  },  
  "noiseOrigin": {  
    "type": "Text",  
    "value": "traffic"  
  },  
  "exposureType": {  
    "type": "Property",  
    "value": "short term exposure"  
  },  
  "buildingsType": {  
    "type": "Text",  
    "value": "residential"  
  },  
  "groundType": {  
    "type": "Text",  
    "value": "concrete"  
  },  
  "wallsType": {  
    "type": "Text",  
    "value": "glass"  
  },  
  "Lamax2": {  
    "type": "Number",  
    "value": 75  
  },  
  "Laeq2": {  
    "type": "Number",  
    "value": 85  
  }  
}  
```  
</details>  
#### NoisePollution NGSI-LD关键值示例  
这里有一个以JSON-LD格式作为key-values的NoisePollution的例子。当使用`options=keyValues`时，这与NGSI-LD兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:NoisePollution:France-NoisePollution-12345_2022-07-01T18:00:00_2022-07-01T00:00:00",  
  "type": "NoisePollution",  
  "Laeq2": 85,  
  "Lamax2": 75,  
  "Lanight": 45,  
  "NoiseAnnoyanceIndex": 3,  
  "address": {  
    "addressCountry": "France",  
    "addressLocality": "Nice",  
    "postalCode": "06200",  
    "type": "PostalAddress"  
  },  
  "buildingsType": "residential",  
  "dataProvider": "IMREDD_UCA_Nice",  
  "dateObservedFrom": "2022-07-01T10:40:01.00Z",  
  "dateObservedTo": "2022-07-01T12:40:01.00Z",  
  "exposureType": "short term exposure",  
  "groundType": "concrete",  
  "location": {  
    "coordinates": [  
      7.2032497427380235,  
      43.68056738083439  
    ],  
    "type": "Point"  
  },  
  "noiseOrigin": "traffic",  
  "wallsType": "glass",  
  "@context": [  
    "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld",  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.Environment/master/context.jsonld"  
  ]  
}  
```  
</details>  
#### NoisePollution NGSI-LD归一化实例  
下面是一个以JSON-LD格式规范化的NoisePollution的例子。当不使用选项时，这与NGSI-LD兼容，并返回单个实体的上下文数据。  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "urn:ngsi-ld:NoisePollution:France-NoisePollution-12345_2022-07-01T18:00:00_2022-07-01T00:00:00",  
  "type": "NoisePollution",  
  "address": {  
    "type": "Property",  
    "value": {  
      "addressCountry": "France",  
      "postalCode": "06200",  
      "addressLocality": "Nice",  
      "type": "PostalAddress"  
    }  
  },  
  "location": {  
    "type": "GeoProperty",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        7.2032497427380235,  
        43.68056738083439  
      ]  
    }  
  },  
  "dataProvider": {  
    "type": "Property",  
    "value": "IMREDD_UCA_Nice"  
  },  
  "dateObservedFrom": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2022-07-01T10:40:01.00Z"  
    }  
  },  
  "dateObservedTo": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2022-07-01T12:40:01.00Z"  
    }  
  },  
  "NoiseAnnoyanceIndex": {  
    "type": "Property",  
    "value": 3  
  },  
  "Lanight": {  
    "type": "Property",  
    "value": 45  
  },  
  "noiseOrigin": {  
    "type": "Property",  
    "value": "traffic"  
  },  
  "exposureType": {  
    "type": "Property",  
    "value": "short term exposure"  
  },  
  "buildingsType": {  
    "type": "Property",  
    "value": "residential"  
  },  
  "groundType": {  
    "type": "Property",  
    "value": "concrete"  
  },  
  "wallsType": {  
    "type": "Property",  
    "value": "glass"  
  },  
  "Lamax2": {  
    "type": "Property",  
    "value": 75  
  },  
  "Laeq2": {  
    "type": "Property",  
    "value": 85  
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
参见[常见问题10](https://smartdatamodels.org/index.php/faqs/)，以获得关于如何处理量级单位的答案。  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
