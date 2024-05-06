# LoadArea


_The class is the root or first level in a hierarchical structure for grouping of loads for the purpose of load flow load scaling._





**URI**: [cim:LoadArea](http://iec.ch/TC57/CIM100#LoadArea)<br />
**Type**: Class




```mermaid
 classDiagram
    class LoadArea
    click LoadArea href "../LoadArea"
      EnergyArea <|-- LoadArea
        click EnergyArea href "../EnergyArea"
      
      LoadArea : EnergyArea.ControlArea
        
          LoadArea --> ControlArea : EnergyArea.ControlArea
          click ControlArea href "../ControlArea"
        
      LoadArea : IdentifiedObject.description
        
      LoadArea : IdentifiedObject.energyIdentCodeEic
        
      LoadArea : IdentifiedObject.mRID
        
      LoadArea : IdentifiedObject.name
        
      LoadArea : IdentifiedObject.shortName
        
      LoadArea : LoadArea.SubLoadAreas
        
          LoadArea --> SubLoadArea : LoadArea.SubLoadAreas
          click SubLoadArea href "../SubLoadArea"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [EnergyArea](EnergyArea.md)
        * **LoadArea**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| SubLoadAreas | [cim:LoadArea.SubLoadAreas](http://iec.ch/TC57/CIM100#LoadArea.SubLoadAreas) | 1..* <br />  [SubLoadArea](SubLoadArea.md)  | The SubLoadAreas in the LoadArea | direct |
| ControlArea | [cim:EnergyArea.ControlArea](http://iec.ch/TC57/CIM100#EnergyArea.ControlArea) | 0..1 <br />  [ControlArea](ControlArea.md)  | The control area specification that is used for the load forecast | [EnergyArea](EnergyArea.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SubLoadArea](SubLoadArea.md) | LoadArea | range | [LoadArea](LoadArea.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:LoadArea |
| native | this:LoadArea |




