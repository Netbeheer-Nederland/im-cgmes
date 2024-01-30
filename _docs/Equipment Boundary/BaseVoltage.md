# BaseVoltage


_Defines a system base voltage which is referenced._





**URI**: [cim:BaseVoltage](http://iec.ch/TC57/CIM100#BaseVoltage)<br />
**Type**: Class




```mermaid
 classDiagram
    class BaseVoltage
      IdentifiedObject <|-- BaseVoltage
      
      BaseVoltage : IdentifiedObject.description
        
      BaseVoltage : IdentifiedObject.energyIdentCodeEic
        
      BaseVoltage : IdentifiedObject.mRID
        
      BaseVoltage : IdentifiedObject.name
        
      BaseVoltage : BaseVoltage.nominalVoltage
        
          BaseVoltage --> Voltage : BaseVoltage.nominalVoltage
        
      BaseVoltage : IdentifiedObject.shortName
        
      BaseVoltage : BaseVoltage.VoltageLevel
        
          BaseVoltage --> VoltageLevel : BaseVoltage.VoltageLevel
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **BaseVoltage**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| nominalVoltage | [cim:BaseVoltage.nominalVoltage](http://iec.ch/TC57/CIM100#BaseVoltage.nominalVoltage) | 1..1 <br />  [Voltage](Voltage.md)  | The power system resource's base voltage | direct |
| VoltageLevel | [cim:BaseVoltage.VoltageLevel](http://iec.ch/TC57/CIM100#BaseVoltage.VoltageLevel) | 0..* <br />  [VoltageLevel](VoltageLevel.md)  | The voltage levels having this base voltage | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [VoltageLevel](VoltageLevel.md) | BaseVoltage | range | [BaseVoltage](BaseVoltage.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:BaseVoltage |
| native | this:BaseVoltage |




