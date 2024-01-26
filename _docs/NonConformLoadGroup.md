# NonConformLoadGroup


_Loads that do not follow a daily and seasonal load variation pattern._





**URI**: [cim:NonConformLoadGroup](http://iec.ch/TC57/CIM100#NonConformLoadGroup)<br />
**Type**: Class




```mermaid
 classDiagram
    class NonConformLoadGroup
      LoadGroup <|-- NonConformLoadGroup
      
      NonConformLoadGroup : IdentifiedObject.description
        
      NonConformLoadGroup : NonConformLoadGroup.EnergyConsumers
        
          NonConformLoadGroup --> NonConformLoad : NonConformLoadGroup.EnergyConsumers
        
      NonConformLoadGroup : IdentifiedObject.energyIdentCodeEic
        
      NonConformLoadGroup : IdentifiedObject.mRID
        
      NonConformLoadGroup : IdentifiedObject.name
        
      NonConformLoadGroup : NonConformLoadGroup.NonConformLoadSchedules
        
          NonConformLoadGroup --> NonConformLoadSchedule : NonConformLoadGroup.NonConformLoadSchedules
        
      NonConformLoadGroup : IdentifiedObject.shortName
        
      NonConformLoadGroup : LoadGroup.SubLoadArea
        
          NonConformLoadGroup --> SubLoadArea : LoadGroup.SubLoadArea
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [LoadGroup](LoadGroup.md)
        * **NonConformLoadGroup**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| EnergyConsumers | [cim:NonConformLoadGroup.EnergyConsumers](http://iec.ch/TC57/CIM100#NonConformLoadGroup.EnergyConsumers) | 1..* <br />  [NonConformLoad](NonConformLoad.md)  | Conform loads assigned to this ConformLoadGroup | direct |
| NonConformLoadSchedules | [cim:NonConformLoadGroup.NonConformLoadSchedules](http://iec.ch/TC57/CIM100#NonConformLoadGroup.NonConformLoadSchedules) | 0..* <br />  [NonConformLoadSchedule](NonConformLoadSchedule.md)  | The NonConformLoadSchedules in the NonConformLoadGroup | direct |
| SubLoadArea | [cim:LoadGroup.SubLoadArea](http://iec.ch/TC57/CIM100#LoadGroup.SubLoadArea) | 1..1 <br />  [SubLoadArea](SubLoadArea.md)  | The SubLoadArea where the Loadgroup belongs | [LoadGroup](LoadGroup.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [NonConformLoad](NonConformLoad.md) | LoadGroup | range | [NonConformLoadGroup](NonConformLoadGroup.md) |
| [NonConformLoadSchedule](NonConformLoadSchedule.md) | NonConformLoadGroup | range | [NonConformLoadGroup](NonConformLoadGroup.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:NonConformLoadGroup |
| native | this:NonConformLoadGroup |




