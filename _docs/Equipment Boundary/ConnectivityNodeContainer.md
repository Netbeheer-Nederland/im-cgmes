# ConnectivityNodeContainer


_A base class for all objects that may contain connectivity nodes or topological nodes._





**URI**: [cim:ConnectivityNodeContainer](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConnectivityNodeContainer
    click ConnectivityNodeContainer href "../ConnectivityNodeContainer"
      PowerSystemResource <|-- ConnectivityNodeContainer
        click PowerSystemResource href "../PowerSystemResource"
      

      ConnectivityNodeContainer <|-- EquipmentContainer
        click EquipmentContainer href "../EquipmentContainer"
      
      
      ConnectivityNodeContainer : ConnectivityNodeContainer.ConnectivityNodes
        
          ConnectivityNodeContainer --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
          click ConnectivityNode href "../ConnectivityNode"
        
      ConnectivityNodeContainer : IdentifiedObject.description
        
      ConnectivityNodeContainer : IdentifiedObject.energyIdentCodeEic
        
      ConnectivityNodeContainer : IdentifiedObject.mRID
        
      ConnectivityNodeContainer : IdentifiedObject.name
        
      ConnectivityNodeContainer : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **ConnectivityNodeContainer**
            * [EquipmentContainer](EquipmentContainer.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | * <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConnectivityNode](ConnectivityNode.md) | ConnectivityNodeContainer | range | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConnectivityNodeContainer |
| native | this:ConnectivityNodeContainer |




