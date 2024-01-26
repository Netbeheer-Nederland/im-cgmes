# LoadGroup


_The class is the third level in a hierarchical structure for grouping of loads for the purpose of load flow load scaling._





**URI**: [cim:LoadGroup](http://iec.ch/TC57/CIM100#LoadGroup)<br />
**Type**: Class




```mermaid
 classDiagram
    class LoadGroup
      IdentifiedObject <|-- LoadGroup
      

      LoadGroup <|-- ConformLoadGroup
      LoadGroup <|-- NonConformLoadGroup
      
      
      LoadGroup : IdentifiedObject.description
        
      LoadGroup : IdentifiedObject.energyIdentCodeEic
        
      LoadGroup : IdentifiedObject.mRID
        
      LoadGroup : IdentifiedObject.name
        
      LoadGroup : IdentifiedObject.shortName
        
      LoadGroup : LoadGroup.SubLoadArea
        
          LoadGroup --> SubLoadArea : LoadGroup.SubLoadArea
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **LoadGroup**
        * [ConformLoadGroup](ConformLoadGroup.md)
        * [NonConformLoadGroup](NonConformLoadGroup.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| SubLoadArea | [cim:LoadGroup.SubLoadArea](http://iec.ch/TC57/CIM100#LoadGroup.SubLoadArea) | 1..1 <br />  [SubLoadArea](SubLoadArea.md)  | The SubLoadArea where the Loadgroup belongs | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SubLoadArea](SubLoadArea.md) | LoadGroups | range | [LoadGroup](LoadGroup.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:LoadGroup |
| native | this:LoadGroup |




