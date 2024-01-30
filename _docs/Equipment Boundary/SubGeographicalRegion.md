# SubGeographicalRegion


_A subset of a geographical region of a power system network model._





**URI**: [cim:SubGeographicalRegion](http://iec.ch/TC57/CIM100#SubGeographicalRegion)<br />
**Type**: Class




```mermaid
 classDiagram
    class SubGeographicalRegion
      IdentifiedObject <|-- SubGeographicalRegion
      
      SubGeographicalRegion : IdentifiedObject.description
        
      SubGeographicalRegion : IdentifiedObject.energyIdentCodeEic
        
      SubGeographicalRegion : SubGeographicalRegion.Lines
        
          SubGeographicalRegion --> Line : SubGeographicalRegion.Lines
        
      SubGeographicalRegion : IdentifiedObject.mRID
        
      SubGeographicalRegion : IdentifiedObject.name
        
      SubGeographicalRegion : SubGeographicalRegion.Region
        
          SubGeographicalRegion --> GeographicalRegion : SubGeographicalRegion.Region
        
      SubGeographicalRegion : IdentifiedObject.shortName
        
      SubGeographicalRegion : SubGeographicalRegion.Substations
        
          SubGeographicalRegion --> Substation : SubGeographicalRegion.Substations
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **SubGeographicalRegion**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Region | [cim:SubGeographicalRegion.Region](http://iec.ch/TC57/CIM100#SubGeographicalRegion.Region) | 1..1 <br />  [GeographicalRegion](GeographicalRegion.md)  | The geographical region which this sub-geographical region is within | direct |
| Lines | [cim:SubGeographicalRegion.Lines](http://iec.ch/TC57/CIM100#SubGeographicalRegion.Lines) | 0..* <br />  [Line](Line.md)  | The lines within the sub-geographical region | direct |
| Substations | [cim:SubGeographicalRegion.Substations](http://iec.ch/TC57/CIM100#SubGeographicalRegion.Substations) | 0..* <br />  [Substation](Substation.md)  | The substations in this sub-geographical region | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [GeographicalRegion](GeographicalRegion.md) | Regions | range | [SubGeographicalRegion](SubGeographicalRegion.md) |
| [Line](Line.md) | Region | range | [SubGeographicalRegion](SubGeographicalRegion.md) |
| [Substation](Substation.md) | Region | range | [SubGeographicalRegion](SubGeographicalRegion.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SubGeographicalRegion |
| native | this:SubGeographicalRegion |




