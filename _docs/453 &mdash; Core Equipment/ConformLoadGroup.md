# ConformLoadGroup


_A group of loads conforming to an allocation pattern._





**URI**: [cim:ConformLoadGroup](http://iec.ch/TC57/CIM100#ConformLoadGroup)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConformLoadGroup
      LoadGroup <|-- ConformLoadGroup
      
      ConformLoadGroup : ConformLoadGroup.ConformLoadSchedules
        
          ConformLoadGroup --> ConformLoadSchedule : ConformLoadGroup.ConformLoadSchedules
        
      ConformLoadGroup : IdentifiedObject.description
        
      ConformLoadGroup : ConformLoadGroup.EnergyConsumers
        
          ConformLoadGroup --> ConformLoad : ConformLoadGroup.EnergyConsumers
        
      ConformLoadGroup : IdentifiedObject.energyIdentCodeEic
        
      ConformLoadGroup : IdentifiedObject.mRID
        
      ConformLoadGroup : IdentifiedObject.name
        
      ConformLoadGroup : IdentifiedObject.shortName
        
      ConformLoadGroup : LoadGroup.SubLoadArea
        
          ConformLoadGroup --> SubLoadArea : LoadGroup.SubLoadArea
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [LoadGroup](LoadGroup.md)
        * **ConformLoadGroup**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ConformLoadSchedules | [cim:ConformLoadGroup.ConformLoadSchedules](http://iec.ch/TC57/CIM100#ConformLoadGroup.ConformLoadSchedules) | 0..* <br />  [ConformLoadSchedule](ConformLoadSchedule.md)  | The ConformLoadSchedules in the ConformLoadGroup | direct |
| EnergyConsumers | [cim:ConformLoadGroup.EnergyConsumers](http://iec.ch/TC57/CIM100#ConformLoadGroup.EnergyConsumers) | 1..* <br />  [ConformLoad](ConformLoad.md)  | Conform loads assigned to this ConformLoadGroup | direct |
| SubLoadArea | [cim:LoadGroup.SubLoadArea](http://iec.ch/TC57/CIM100#LoadGroup.SubLoadArea) | 1..1 <br />  [SubLoadArea](SubLoadArea.md)  | The SubLoadArea where the Loadgroup belongs | [LoadGroup](LoadGroup.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConformLoadSchedule](ConformLoadSchedule.md) | ConformLoadGroup | range | [ConformLoadGroup](ConformLoadGroup.md) |
| [ConformLoad](ConformLoad.md) | LoadGroup | range | [ConformLoadGroup](ConformLoadGroup.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConformLoadGroup |
| native | this:ConformLoadGroup |




