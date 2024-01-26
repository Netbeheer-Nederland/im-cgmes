# DCEquipmentContainer


_A modelling construct to provide a root class for containment of DC as well as AC equipment. The class differ from the EquipmentContaner for AC in that it may also contain DCNode-s. Hence it can contain both AC and DC equipment._





**URI**: [cim:DCEquipmentContainer](http://iec.ch/TC57/CIM100#DCEquipmentContainer)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCEquipmentContainer
      EquipmentContainer <|-- DCEquipmentContainer
      

      DCEquipmentContainer <|-- DCConverterUnit
      DCEquipmentContainer <|-- DCLine
      
      
      DCEquipmentContainer : ConnectivityNodeContainer.ConnectivityNodes
        
          DCEquipmentContainer --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
        
      DCEquipmentContainer : DCEquipmentContainer.DCNodes
        
          DCEquipmentContainer --> DCNode : DCEquipmentContainer.DCNodes
        
      DCEquipmentContainer : IdentifiedObject.description
        
      DCEquipmentContainer : IdentifiedObject.energyIdentCodeEic
        
      DCEquipmentContainer : EquipmentContainer.Equipments
        
          DCEquipmentContainer --> Equipment : EquipmentContainer.Equipments
        
      DCEquipmentContainer : IdentifiedObject.mRID
        
      DCEquipmentContainer : IdentifiedObject.name
        
      DCEquipmentContainer : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * [EquipmentContainer](EquipmentContainer.md)
                * **DCEquipmentContainer**
                    * [DCConverterUnit](DCConverterUnit.md)
                    * [DCLine](DCLine.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DCNodes | [cim:DCEquipmentContainer.DCNodes](http://iec.ch/TC57/CIM100#DCEquipmentContainer.DCNodes) | 0..* <br />  [DCNode](DCNode.md)  | The DC nodes contained in the DC equipment container | direct |
| Equipments | [cim:EquipmentContainer.Equipments](http://iec.ch/TC57/CIM100#EquipmentContainer.Equipments) | 0..* <br />  [Equipment](Equipment.md)  | Contained equipment | [EquipmentContainer](EquipmentContainer.md) |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | 0..* <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCNode](DCNode.md) | DCEquipmentContainer | range | [DCEquipmentContainer](DCEquipmentContainer.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCEquipmentContainer |
| native | this:DCEquipmentContainer |




