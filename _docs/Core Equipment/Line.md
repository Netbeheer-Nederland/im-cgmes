# Line


_Contains equipment beyond a substation belonging to a power transmission line._





**URI**: [cim:Line](http://iec.ch/TC57/CIM100#Line)<br />
**Type**: Class




```mermaid
 classDiagram
    class Line
    click Line href "../Line"
      EquipmentContainer <|-- Line
        click EquipmentContainer href "../EquipmentContainer"
      
      Line : ConnectivityNodeContainer.ConnectivityNodes
        
          Line --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
          click ConnectivityNode href "../ConnectivityNode"
        
      Line : IdentifiedObject.description
        
      Line : IdentifiedObject.energyIdentCodeEic
        
      Line : EquipmentContainer.Equipments
        
          Line --> Equipment : EquipmentContainer.Equipments
          click Equipment href "../Equipment"
        
      Line : IdentifiedObject.mRID
        
      Line : IdentifiedObject.name
        
      Line : Line.Region
        
          Line --> SubGeographicalRegion : Line.Region
          click SubGeographicalRegion href "../SubGeographicalRegion"
        
      Line : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * [EquipmentContainer](EquipmentContainer.md)
                * **Line**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Region | [cim:Line.Region](http://iec.ch/TC57/CIM100#Line.Region) | 0..1 <br />  [SubGeographicalRegion](SubGeographicalRegion.md)  | The sub-geographical region of the line | direct |
| Equipments | [cim:EquipmentContainer.Equipments](http://iec.ch/TC57/CIM100#EquipmentContainer.Equipments) | * <br />  [Equipment](Equipment.md)  | Contained equipment | [EquipmentContainer](EquipmentContainer.md) |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | * <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SubGeographicalRegion](SubGeographicalRegion.md) | Lines | range | [Line](Line.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Line |
| native | this:Line |




