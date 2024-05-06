# Bay


_A collection of power system resources (within a given substation) including conducting equipment, protection relays, measurements, and telemetry.  A bay typically represents a physical grouping related to modularization of equipment._





**URI**: [cim:Bay](http://iec.ch/TC57/CIM100#Bay)<br />
**Type**: Class




```mermaid
 classDiagram
    class Bay
    click Bay href "../Bay"
      EquipmentContainer <|-- Bay
        click EquipmentContainer href "../EquipmentContainer"
      
      Bay : ConnectivityNodeContainer.ConnectivityNodes
        
          Bay --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
          click ConnectivityNode href "../ConnectivityNode"
        
      Bay : IdentifiedObject.description
        
      Bay : IdentifiedObject.energyIdentCodeEic
        
      Bay : EquipmentContainer.Equipments
        
          Bay --> Equipment : EquipmentContainer.Equipments
          click Equipment href "../Equipment"
        
      Bay : IdentifiedObject.mRID
        
      Bay : IdentifiedObject.name
        
      Bay : IdentifiedObject.shortName
        
      Bay : Bay.VoltageLevel
        
          Bay --> VoltageLevel : Bay.VoltageLevel
          click VoltageLevel href "../VoltageLevel"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * [EquipmentContainer](EquipmentContainer.md)
                * **Bay**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| VoltageLevel | [cim:Bay.VoltageLevel](http://iec.ch/TC57/CIM100#Bay.VoltageLevel) | 1 <br />  [VoltageLevel](VoltageLevel.md)  | The voltage level containing this bay | direct |
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
| [VoltageLevel](VoltageLevel.md) | Bays | range | [Bay](Bay.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Bay |
| native | this:Bay |




