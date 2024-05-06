# EnergyArea


_Describes an area having energy production or consumption.  Specializations are intended to support the load allocation function as typically required in energy management systems or planning studies to allocate hypothesized load levels to individual load points for power flow analysis.  Often the energy area can be linked to both measured and forecast load levels._





**URI**: [cim:EnergyArea](http://iec.ch/TC57/CIM100#EnergyArea)<br />
**Type**: Class




```mermaid
 classDiagram
    class EnergyArea
    click EnergyArea href "../EnergyArea"
      IdentifiedObject <|-- EnergyArea
        click IdentifiedObject href "../IdentifiedObject"
      

      EnergyArea <|-- LoadArea
        click LoadArea href "../LoadArea"
      EnergyArea <|-- SubLoadArea
        click SubLoadArea href "../SubLoadArea"
      
      
      EnergyArea : EnergyArea.ControlArea
        
          EnergyArea --> ControlArea : EnergyArea.ControlArea
          click ControlArea href "../ControlArea"
        
      EnergyArea : IdentifiedObject.description
        
      EnergyArea : IdentifiedObject.energyIdentCodeEic
        
      EnergyArea : IdentifiedObject.mRID
        
      EnergyArea : IdentifiedObject.name
        
      EnergyArea : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **EnergyArea**
        * [LoadArea](LoadArea.md)
        * [SubLoadArea](SubLoadArea.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ControlArea | [cim:EnergyArea.ControlArea](http://iec.ch/TC57/CIM100#EnergyArea.ControlArea) | 0..1 <br />  [ControlArea](ControlArea.md)  | The control area specification that is used for the load forecast | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ControlArea](ControlArea.md) | EnergyArea | range | [EnergyArea](EnergyArea.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EnergyArea |
| native | this:EnergyArea |




