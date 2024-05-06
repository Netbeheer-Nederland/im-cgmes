# WindPowerPlant


_Wind power plant._





**URI**: [eu:WindPowerPlant](http://iec.ch/TC57/CIM100-European#WindPowerPlant)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindPowerPlant
    click WindPowerPlant href "../WindPowerPlant"
      PowerSystemResource <|-- WindPowerPlant
        click PowerSystemResource href "../PowerSystemResource"
      
      WindPowerPlant : IdentifiedObject.description
        
      WindPowerPlant : IdentifiedObject.energyIdentCodeEic
        
      WindPowerPlant : IdentifiedObject.mRID
        
      WindPowerPlant : IdentifiedObject.name
        
      WindPowerPlant : IdentifiedObject.shortName
        
      WindPowerPlant : WindPowerPlant.WindGeneratingUnits
        
          WindPowerPlant --> WindGeneratingUnit : WindPowerPlant.WindGeneratingUnits
          click WindGeneratingUnit href "../WindGeneratingUnit"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **WindPowerPlant**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindGeneratingUnits | [eu:WindPowerPlant.WindGeneratingUnits](http://iec.ch/TC57/CIM100-European#WindPowerPlant.WindGeneratingUnits) | * <br />  [WindGeneratingUnit](WindGeneratingUnit.md)  | A wind generating unit or units may be a member of a wind power plant | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindGeneratingUnit](WindGeneratingUnit.md) | WindPowerPlant | range | [WindPowerPlant](WindPowerPlant.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | eu:WindPowerPlant |
| native | this:WindPowerPlant |




