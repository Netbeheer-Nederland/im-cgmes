# EquipmentContainer


_A modelling construct to provide a root class for containing equipment._





**URI**: [cim:EquipmentContainer](http://iec.ch/TC57/CIM100#EquipmentContainer)<br />
**Type**: Class




```mermaid
 classDiagram
    class EquipmentContainer
    click EquipmentContainer href "../EquipmentContainer"
      ConnectivityNodeContainer <|-- EquipmentContainer
        click ConnectivityNodeContainer href "../ConnectivityNodeContainer"
      

      EquipmentContainer <|-- Bay
        click Bay href "../Bay"
      EquipmentContainer <|-- Line
        click Line href "../Line"
      EquipmentContainer <|-- Substation
        click Substation href "../Substation"
      EquipmentContainer <|-- VoltageLevel
        click VoltageLevel href "../VoltageLevel"
      
      
      EquipmentContainer : ConnectivityNodeContainer.ConnectivityNodes
        
          EquipmentContainer --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
          click ConnectivityNode href "../ConnectivityNode"
        
      EquipmentContainer : IdentifiedObject.description
        
      EquipmentContainer : IdentifiedObject.energyIdentCodeEic
        
      EquipmentContainer : EquipmentContainer.Equipments
        
          EquipmentContainer --> Equipment : EquipmentContainer.Equipments
          click Equipment href "../Equipment"
        
      EquipmentContainer : IdentifiedObject.mRID
        
      EquipmentContainer : IdentifiedObject.name
        
      EquipmentContainer : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * **EquipmentContainer**
                * [Bay](Bay.md)
                * [Line](Line.md)
                * [Substation](Substation.md)
                * [VoltageLevel](VoltageLevel.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Equipments | [cim:EquipmentContainer.Equipments](http://iec.ch/TC57/CIM100#EquipmentContainer.Equipments) | * <br />  [Equipment](Equipment.md)  | Contained equipment | direct |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | * <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConductingEquipment](ConductingEquipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Connector](Connector.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Equipment](Equipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Junction](Junction.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EquipmentContainer |
| native | this:EquipmentContainer |




