# CombinedCyclePlant


_A set of combustion turbines and steam turbines where the exhaust heat from the combustion turbines is recovered to make steam for the steam turbines, resulting in greater overall plant efficiency._





**URI**: [cim:CombinedCyclePlant](http://iec.ch/TC57/CIM100#CombinedCyclePlant)<br />
**Type**: Class




```mermaid
 classDiagram
    class CombinedCyclePlant
    click CombinedCyclePlant href "../CombinedCyclePlant"
      PowerSystemResource <|-- CombinedCyclePlant
        click PowerSystemResource href "../PowerSystemResource"
      
      CombinedCyclePlant : IdentifiedObject.description
        
      CombinedCyclePlant : IdentifiedObject.energyIdentCodeEic
        
      CombinedCyclePlant : IdentifiedObject.mRID
        
      CombinedCyclePlant : IdentifiedObject.name
        
      CombinedCyclePlant : IdentifiedObject.shortName
        
      CombinedCyclePlant : CombinedCyclePlant.ThermalGeneratingUnits
        
          CombinedCyclePlant --> ThermalGeneratingUnit : CombinedCyclePlant.ThermalGeneratingUnits
          click ThermalGeneratingUnit href "../ThermalGeneratingUnit"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **CombinedCyclePlant**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ThermalGeneratingUnits | [cim:CombinedCyclePlant.ThermalGeneratingUnits](http://iec.ch/TC57/CIM100#CombinedCyclePlant.ThermalGeneratingUnits) | * <br />  [ThermalGeneratingUnit](ThermalGeneratingUnit.md)  | A thermal generating unit may be a member of a combined cycle plant | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | CombinedCyclePlant | range | [CombinedCyclePlant](CombinedCyclePlant.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CombinedCyclePlant |
| native | this:CombinedCyclePlant |




