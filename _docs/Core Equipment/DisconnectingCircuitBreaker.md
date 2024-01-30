# DisconnectingCircuitBreaker


_A circuit breaking device including disconnecting function, eliminating the need for separate disconnectors._





**URI**: [cim:DisconnectingCircuitBreaker](http://iec.ch/TC57/CIM100#DisconnectingCircuitBreaker)<br />
**Type**: Class




```mermaid
 classDiagram
    class DisconnectingCircuitBreaker
      Breaker <|-- DisconnectingCircuitBreaker
      
      DisconnectingCircuitBreaker : Equipment.aggregate
        
      DisconnectingCircuitBreaker : ConductingEquipment.BaseVoltage
        
          DisconnectingCircuitBreaker --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      DisconnectingCircuitBreaker : IdentifiedObject.description
        
      DisconnectingCircuitBreaker : IdentifiedObject.energyIdentCodeEic
        
      DisconnectingCircuitBreaker : Equipment.EquipmentContainer
        
          DisconnectingCircuitBreaker --> EquipmentContainer : Equipment.EquipmentContainer
        
      DisconnectingCircuitBreaker : IdentifiedObject.mRID
        
      DisconnectingCircuitBreaker : IdentifiedObject.name
        
      DisconnectingCircuitBreaker : Equipment.normallyInService
        
      DisconnectingCircuitBreaker : Switch.normalOpen
        
      DisconnectingCircuitBreaker : Equipment.OperationalLimitSet
        
          DisconnectingCircuitBreaker --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      DisconnectingCircuitBreaker : Switch.ratedCurrent
        
          DisconnectingCircuitBreaker --> CurrentFlow : Switch.ratedCurrent
        
      DisconnectingCircuitBreaker : Switch.retained
        
      DisconnectingCircuitBreaker : IdentifiedObject.shortName
        
      DisconnectingCircuitBreaker : Switch.SwitchSchedules
        
          DisconnectingCircuitBreaker --> SwitchSchedule : Switch.SwitchSchedules
        
      DisconnectingCircuitBreaker : ConductingEquipment.Terminals
        
          DisconnectingCircuitBreaker --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [Switch](Switch.md)
                    * [ProtectedSwitch](ProtectedSwitch.md)
                        * [Breaker](Breaker.md)
                            * **DisconnectingCircuitBreaker**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| normalOpen | [cim:Switch.normalOpen](http://iec.ch/TC57/CIM100#Switch.normalOpen) | 1..1 <br />  boolean  | The attribute is used in cases when no Measurement for the status value is pr... | [Switch](Switch.md) |
| ratedCurrent | [cim:Switch.ratedCurrent](http://iec.ch/TC57/CIM100#Switch.ratedCurrent) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The maximum continuous current carrying capacity in amps governed by the devi... | [Switch](Switch.md) |
| retained | [cim:Switch.retained](http://iec.ch/TC57/CIM100#Switch.retained) | 1..1 <br />  boolean  | Branch is retained in the topological solution | [Switch](Switch.md) |
| SwitchSchedules | [cim:Switch.SwitchSchedules](http://iec.ch/TC57/CIM100#Switch.SwitchSchedules) | 0..* <br />  [SwitchSchedule](SwitchSchedule.md)  | A Switch can be associated with SwitchSchedules | [Switch](Switch.md) |
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









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DisconnectingCircuitBreaker |
| native | this:DisconnectingCircuitBreaker |




