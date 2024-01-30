# ConductingEquipment


_The parts of the AC power system that are designed to carry current or that are conductively connected through terminals._





**URI**: [cim:ConductingEquipment](http://iec.ch/TC57/CIM100#ConductingEquipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConductingEquipment
      Equipment <|-- ConductingEquipment
      

      ConductingEquipment <|-- Connector
      
      
      ConductingEquipment : IdentifiedObject.description
        
      ConductingEquipment : IdentifiedObject.energyIdentCodeEic
        
      ConductingEquipment : Equipment.EquipmentContainer
        
          ConductingEquipment --> EquipmentContainer : Equipment.EquipmentContainer
        
      ConductingEquipment : IdentifiedObject.mRID
        
      ConductingEquipment : IdentifiedObject.name
        
      ConductingEquipment : IdentifiedObject.shortName
        
      ConductingEquipment : ConductingEquipment.Terminals
        
          ConductingEquipment --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **ConductingEquipment**
                * [Connector](Connector.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | direct |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Terminal](Terminal.md) | ConductingEquipment | range | [ConductingEquipment](ConductingEquipment.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConductingEquipment |
| native | this:ConductingEquipment |




