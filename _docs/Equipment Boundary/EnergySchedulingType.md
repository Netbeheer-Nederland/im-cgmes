# EnergySchedulingType


_Used to define the type of generation for scheduling purposes._





**URI**: [cim:EnergySchedulingType](http://iec.ch/TC57/CIM100#EnergySchedulingType)<br />
**Type**: Class




```mermaid
 classDiagram
    class EnergySchedulingType
    click EnergySchedulingType href "../EnergySchedulingType"
      IdentifiedObject <|-- EnergySchedulingType
        click IdentifiedObject href "../IdentifiedObject"
      
      EnergySchedulingType : IdentifiedObject.description
        
      EnergySchedulingType : IdentifiedObject.energyIdentCodeEic
        
      EnergySchedulingType : IdentifiedObject.mRID
        
      EnergySchedulingType : IdentifiedObject.name
        
      EnergySchedulingType : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **EnergySchedulingType**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EnergySchedulingType |
| native | this:EnergySchedulingType |




