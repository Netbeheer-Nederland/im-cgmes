# Switch


_A generic device designed to close, or open, or both, one or more electric circuits.  All switches are two terminal devices including grounding switches. The ACDCTerminal.connected at the two sides of the switch shall not be considered for assessing switch connectivity, i.e. only Switch.open, .normalOpen and .locked are relevant._





**URI**: [cim:Switch](http://iec.ch/TC57/CIM100#Switch)<br />
**Type**: Class




```mermaid
 classDiagram
    class Switch
      ConductingEquipment <|-- Switch
      

      Switch <|-- Cut
      Switch <|-- Disconnector
      Switch <|-- Fuse
      Switch <|-- GroundDisconnector
      Switch <|-- Jumper
      Switch <|-- ProtectedSwitch
      
      
      Switch : Equipment.aggregate
        
      Switch : ConductingEquipment.BaseVoltage
        
          Switch --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      Switch : IdentifiedObject.description
        
      Switch : IdentifiedObject.energyIdentCodeEic
        
      Switch : Equipment.EquipmentContainer
        
          Switch --> EquipmentContainer : Equipment.EquipmentContainer
        
      Switch : IdentifiedObject.mRID
        
      Switch : IdentifiedObject.name
        
      Switch : Equipment.normallyInService
        
      Switch : Switch.normalOpen
        
      Switch : Equipment.OperationalLimitSet
        
          Switch --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      Switch : Switch.ratedCurrent
        
          Switch --> CurrentFlow : Switch.ratedCurrent
        
      Switch : Switch.retained
        
      Switch : IdentifiedObject.shortName
        
      Switch : Switch.SwitchSchedules
        
          Switch --> SwitchSchedule : Switch.SwitchSchedules
        
      Switch : ConductingEquipment.Terminals
        
          Switch --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **Switch**
                    * [Cut](Cut.md)
                    * [Disconnector](Disconnector.md)
                    * [Fuse](Fuse.md)
                    * [GroundDisconnector](GroundDisconnector.md)
                    * [Jumper](Jumper.md)
                    * [ProtectedSwitch](ProtectedSwitch.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| normalOpen | [cim:Switch.normalOpen](http://iec.ch/TC57/CIM100#Switch.normalOpen) | 1..1 <br />  boolean  | The attribute is used in cases when no Measurement for the status value is pr... | direct |
| ratedCurrent | [cim:Switch.ratedCurrent](http://iec.ch/TC57/CIM100#Switch.ratedCurrent) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The maximum continuous current carrying capacity in amps governed by the devi... | direct |
| retained | [cim:Switch.retained](http://iec.ch/TC57/CIM100#Switch.retained) | 1..1 <br />  boolean  | Branch is retained in the topological solution | direct |
| SwitchSchedules | [cim:Switch.SwitchSchedules](http://iec.ch/TC57/CIM100#Switch.SwitchSchedules) | 0..* <br />  [SwitchSchedule](SwitchSchedule.md)  | A Switch can be associated with SwitchSchedules | direct |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | 0..* <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SwitchSchedule](SwitchSchedule.md) | Switch | range | [Switch](Switch.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Switch |
| native | this:Switch |




