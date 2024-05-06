# GeographicalRegion


_A geographical region of a power system network model._





**URI**: [cim:GeographicalRegion](http://iec.ch/TC57/CIM100#GeographicalRegion)<br />
**Type**: Class




```mermaid
 classDiagram
    class GeographicalRegion
    click GeographicalRegion href "../GeographicalRegion"
      IdentifiedObject <|-- GeographicalRegion
        click IdentifiedObject href "../IdentifiedObject"
      
      GeographicalRegion : IdentifiedObject.description
        
      GeographicalRegion : IdentifiedObject.energyIdentCodeEic
        
      GeographicalRegion : IdentifiedObject.mRID
        
      GeographicalRegion : IdentifiedObject.name
        
      GeographicalRegion : GeographicalRegion.Regions
        
          GeographicalRegion --> SubGeographicalRegion : GeographicalRegion.Regions
          click SubGeographicalRegion href "../SubGeographicalRegion"
        
      GeographicalRegion : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **GeographicalRegion**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Regions | [cim:GeographicalRegion.Regions](http://iec.ch/TC57/CIM100#GeographicalRegion.Regions) | * <br />  [SubGeographicalRegion](SubGeographicalRegion.md)  | All sub-geographical regions within this geographical region | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SubGeographicalRegion](SubGeographicalRegion.md) | Region | range | [GeographicalRegion](GeographicalRegion.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:GeographicalRegion |
| native | this:GeographicalRegion |




