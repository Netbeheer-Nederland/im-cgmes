# Substation


_A collection of equipment for purposes other than generation or utilization, through which electric energy in bulk is passed for the purposes of switching or modifying its characteristics._





**URI**: [cim:Substation](http://iec.ch/TC57/CIM100#Substation)<br />
**Type**: Class




```mermaid
 classDiagram
    class Substation
      EquipmentContainer <|-- Substation
      
      Substation : ConnectivityNodeContainer.ConnectivityNodes
        
          Substation --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
        
      Substation : IdentifiedObject.description
        
      Substation : IdentifiedObject.energyIdentCodeEic
        
      Substation : EquipmentContainer.Equipments
        
          Substation --> Equipment : EquipmentContainer.Equipments
        
      Substation : IdentifiedObject.mRID
        
      Substation : IdentifiedObject.name
        
      Substation : Substation.Region
        
          Substation --> SubGeographicalRegion : Substation.Region
        
      Substation : IdentifiedObject.shortName
        
      Substation : Substation.VoltageLevels
        
          Substation --> VoltageLevel : Substation.VoltageLevels
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * [EquipmentContainer](EquipmentContainer.md)
                * **Substation**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Region | [cim:Substation.Region](http://iec.ch/TC57/CIM100#Substation.Region) | 1..1 <br />  [SubGeographicalRegion](SubGeographicalRegion.md)  | The SubGeographicalRegion containing the substation | direct |
| VoltageLevels | [cim:Substation.VoltageLevels](http://iec.ch/TC57/CIM100#Substation.VoltageLevels) | 0..* <br />  [VoltageLevel](VoltageLevel.md)  | The voltage levels within this substation | direct |
| Equipments | [cim:EquipmentContainer.Equipments](http://iec.ch/TC57/CIM100#EquipmentContainer.Equipments) | 0..* <br />  [Equipment](Equipment.md)  | Contained equipment | [EquipmentContainer](EquipmentContainer.md) |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | 0..* <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SubGeographicalRegion](SubGeographicalRegion.md) | Substations | range | [Substation](Substation.md) |
| [VoltageLevel](VoltageLevel.md) | Substation | range | [Substation](Substation.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Substation |
| native | this:Substation |




