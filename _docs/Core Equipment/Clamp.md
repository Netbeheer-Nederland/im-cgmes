# Clamp


_A Clamp is a galvanic connection at a line segment where other equipment is connected. A Clamp does not cut the line segment. _

_A Clamp is ConductingEquipment and has one Terminal with an associated ConnectivityNode. Any other ConductingEquipment can be connected to the Clamp ConnectivityNode._





**URI**: [cim:Clamp](http://iec.ch/TC57/CIM100#Clamp)<br />
**Type**: Class




```mermaid
 classDiagram
    class Clamp
    click Clamp href "../Clamp"
      ConductingEquipment <|-- Clamp
        click ConductingEquipment href "../ConductingEquipment"
      
      Clamp : Clamp.ACLineSegment
        
          Clamp --> ACLineSegment : Clamp.ACLineSegment
          click ACLineSegment href "../ACLineSegment"
        
      Clamp : Equipment.aggregate
        
      Clamp : ConductingEquipment.BaseVoltage
        
          Clamp --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      Clamp : IdentifiedObject.description
        
      Clamp : IdentifiedObject.energyIdentCodeEic
        
      Clamp : Equipment.EquipmentContainer
        
          Clamp --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      Clamp : Clamp.lengthFromTerminal1
        
          Clamp --> Length : Clamp.lengthFromTerminal1
          click Length href "../Length"
        
      Clamp : IdentifiedObject.mRID
        
      Clamp : IdentifiedObject.name
        
      Clamp : Equipment.normallyInService
        
      Clamp : Equipment.OperationalLimitSet
        
          Clamp --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      Clamp : IdentifiedObject.shortName
        
      Clamp : ConductingEquipment.Terminals
        
          Clamp --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **Clamp**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ACLineSegment | [cim:Clamp.ACLineSegment](http://iec.ch/TC57/CIM100#Clamp.ACLineSegment) | 1 <br />  [ACLineSegment](ACLineSegment.md)  | The line segment to which the clamp is connected | direct |
| lengthFromTerminal1 | [cim:Clamp.lengthFromTerminal1](http://iec.ch/TC57/CIM100#Clamp.lengthFromTerminal1) | 0..1 <br />  [Length](Length.md)  | The length to the place where the clamp is located starting from side one of ... | direct |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | * <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACLineSegment](ACLineSegment.md) | Clamp | range | [Clamp](Clamp.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Clamp |
| native | this:Clamp |




