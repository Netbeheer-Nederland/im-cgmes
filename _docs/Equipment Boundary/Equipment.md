# Equipment


_The parts of a power system that are physical devices, electronic or mechanical._





**URI**: [cim:Equipment](http://iec.ch/TC57/CIM100#Equipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class Equipment
      PowerSystemResource <|-- Equipment
      

      Equipment <|-- ConductingEquipment
      
      
      Equipment : IdentifiedObject.description
        
      Equipment : IdentifiedObject.energyIdentCodeEic
        
      Equipment : Equipment.EquipmentContainer
        
          Equipment --> EquipmentContainer : Equipment.EquipmentContainer
        
      Equipment : IdentifiedObject.mRID
        
      Equipment : IdentifiedObject.name
        
      Equipment : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **Equipment**
            * [ConductingEquipment](ConductingEquipment.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Bay](Bay.md) | Equipments | range | [Equipment](Equipment.md) |
| [EquipmentContainer](EquipmentContainer.md) | Equipments | range | [Equipment](Equipment.md) |
| [Line](Line.md) | Equipments | range | [Equipment](Equipment.md) |
| [Substation](Substation.md) | Equipments | range | [Equipment](Equipment.md) |
| [VoltageLevel](VoltageLevel.md) | Equipments | range | [Equipment](Equipment.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Equipment |
| native | this:Equipment |




