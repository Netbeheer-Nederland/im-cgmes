# RatioTapChangerTable


_Describes a curve for how the voltage magnitude and impedance varies with the tap step._





**URI**: [cim:RatioTapChangerTable](http://iec.ch/TC57/CIM100#RatioTapChangerTable)<br />
**Type**: Class




```mermaid
 classDiagram
    class RatioTapChangerTable
      IdentifiedObject <|-- RatioTapChangerTable
      
      RatioTapChangerTable : IdentifiedObject.description
        
      RatioTapChangerTable : IdentifiedObject.energyIdentCodeEic
        
      RatioTapChangerTable : IdentifiedObject.mRID
        
      RatioTapChangerTable : IdentifiedObject.name
        
      RatioTapChangerTable : RatioTapChangerTable.RatioTapChanger
        
          RatioTapChangerTable --> RatioTapChanger : RatioTapChangerTable.RatioTapChanger
        
      RatioTapChangerTable : RatioTapChangerTable.RatioTapChangerTablePoint
        
          RatioTapChangerTable --> RatioTapChangerTablePoint : RatioTapChangerTable.RatioTapChangerTablePoint
        
      RatioTapChangerTable : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **RatioTapChangerTable**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RatioTapChanger | [cim:RatioTapChangerTable.RatioTapChanger](http://iec.ch/TC57/CIM100#RatioTapChangerTable.RatioTapChanger) | 0..* <br />  [RatioTapChanger](RatioTapChanger.md)  | The ratio tap changer of this tap ratio table | direct |
| RatioTapChangerTablePoint | [cim:RatioTapChangerTable.RatioTapChangerTablePoint](http://iec.ch/TC57/CIM100#RatioTapChangerTable.RatioTapChangerTablePoint) | 1..* <br />  [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md)  | Points of this table | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RatioTapChanger](RatioTapChanger.md) | RatioTapChangerTable | range | [RatioTapChangerTable](RatioTapChangerTable.md) |
| [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md) | RatioTapChangerTable | range | [RatioTapChangerTable](RatioTapChangerTable.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RatioTapChangerTable |
| native | this:RatioTapChangerTable |




