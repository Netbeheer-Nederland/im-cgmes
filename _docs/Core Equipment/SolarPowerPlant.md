# SolarPowerPlant


_Solar power plant._





**URI**: [eu:SolarPowerPlant](http://iec.ch/TC57/CIM100-European#SolarPowerPlant)<br />
**Type**: Class




```mermaid
 classDiagram
    class SolarPowerPlant
    click SolarPowerPlant href "../SolarPowerPlant"
      PowerSystemResource <|-- SolarPowerPlant
        click PowerSystemResource href "../PowerSystemResource"
      
      SolarPowerPlant : IdentifiedObject.description
        
      SolarPowerPlant : IdentifiedObject.energyIdentCodeEic
        
      SolarPowerPlant : IdentifiedObject.mRID
        
      SolarPowerPlant : IdentifiedObject.name
        
      SolarPowerPlant : IdentifiedObject.shortName
        
      SolarPowerPlant : SolarPowerPlant.SolarGeneratingUnits
        
          SolarPowerPlant --> SolarGeneratingUnit : SolarPowerPlant.SolarGeneratingUnits
          click SolarGeneratingUnit href "../SolarGeneratingUnit"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **SolarPowerPlant**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| SolarGeneratingUnits | [eu:SolarPowerPlant.SolarGeneratingUnits](http://iec.ch/TC57/CIM100-European#SolarPowerPlant.SolarGeneratingUnits) | * <br />  [SolarGeneratingUnit](SolarGeneratingUnit.md)  | A solar generating unit or units may be a member of a solar power plant | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SolarGeneratingUnit](SolarGeneratingUnit.md) | SolarPowerPlant | range | [SolarPowerPlant](SolarPowerPlant.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | eu:SolarPowerPlant |
| native | this:SolarPowerPlant |




