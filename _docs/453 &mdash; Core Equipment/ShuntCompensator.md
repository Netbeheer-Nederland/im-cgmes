# ShuntCompensator


_A shunt capacitor or reactor or switchable bank of shunt capacitors or reactors. A section of a shunt compensator is an individual capacitor or reactor. A negative value for bPerSection indicates that the compensator is a reactor. ShuntCompensator is a single terminal device.  Ground is implied._





**URI**: [cim:ShuntCompensator](http://iec.ch/TC57/CIM100#ShuntCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class ShuntCompensator
      RegulatingCondEq <|-- ShuntCompensator
      

      ShuntCompensator <|-- LinearShuntCompensator
      ShuntCompensator <|-- NonlinearShuntCompensator
      
      
      ShuntCompensator : Equipment.aggregate
        
      ShuntCompensator : ShuntCompensator.aVRDelay
        
          ShuntCompensator --> Seconds : ShuntCompensator.aVRDelay
        
      ShuntCompensator : ConductingEquipment.BaseVoltage
        
          ShuntCompensator --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      ShuntCompensator : IdentifiedObject.description
        
      ShuntCompensator : IdentifiedObject.energyIdentCodeEic
        
      ShuntCompensator : Equipment.EquipmentContainer
        
          ShuntCompensator --> EquipmentContainer : Equipment.EquipmentContainer
        
      ShuntCompensator : ShuntCompensator.grounded
        
      ShuntCompensator : ShuntCompensator.maximumSections
        
      ShuntCompensator : IdentifiedObject.mRID
        
      ShuntCompensator : IdentifiedObject.name
        
      ShuntCompensator : ShuntCompensator.nomU
        
          ShuntCompensator --> Voltage : ShuntCompensator.nomU
        
      ShuntCompensator : Equipment.normallyInService
        
      ShuntCompensator : ShuntCompensator.normalSections
        
      ShuntCompensator : Equipment.OperationalLimitSet
        
          ShuntCompensator --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      ShuntCompensator : RegulatingCondEq.RegulatingControl
        
          ShuntCompensator --> RegulatingControl : RegulatingCondEq.RegulatingControl
        
      ShuntCompensator : IdentifiedObject.shortName
        
      ShuntCompensator : ConductingEquipment.Terminals
        
          ShuntCompensator --> Terminal : ConductingEquipment.Terminals
        
      ShuntCompensator : ShuntCompensator.voltageSensitivity
        
          ShuntCompensator --> VoltagePerReactivePower : ShuntCompensator.voltageSensitivity
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * **ShuntCompensator**
                            * [LinearShuntCompensator](LinearShuntCompensator.md)
                            * [NonlinearShuntCompensator](NonlinearShuntCompensator.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| aVRDelay | [cim:ShuntCompensator.aVRDelay](http://iec.ch/TC57/CIM100#ShuntCompensator.aVRDelay) | 0..1 <br />  [Seconds](Seconds.md)  | An automatic voltage regulation delay (AVRDelay) which is the time delay from... | direct |
| grounded | [cim:ShuntCompensator.grounded](http://iec.ch/TC57/CIM100#ShuntCompensator.grounded) | 0..1 <br />  boolean  | Used for Yn and Zn connections | direct |
| maximumSections | [cim:ShuntCompensator.maximumSections](http://iec.ch/TC57/CIM100#ShuntCompensator.maximumSections) | 1..1 <br />  integer  | The maximum number of sections that may be switched in | direct |
| nomU | [cim:ShuntCompensator.nomU](http://iec.ch/TC57/CIM100#ShuntCompensator.nomU) | 1..1 <br />  [Voltage](Voltage.md)  | The voltage at which the nominal reactive power may be calculated | direct |
| normalSections | [cim:ShuntCompensator.normalSections](http://iec.ch/TC57/CIM100#ShuntCompensator.normalSections) | 1..1 <br />  integer  | The normal number of sections switched in | direct |
| voltageSensitivity | [cim:ShuntCompensator.voltageSensitivity](http://iec.ch/TC57/CIM100#ShuntCompensator.voltageSensitivity) | 0..1 <br />  [VoltagePerReactivePower](VoltagePerReactivePower.md)  | Voltage sensitivity required for the device to regulate the bus voltage, in v... | direct |
| RegulatingControl | [cim:RegulatingCondEq.RegulatingControl](http://iec.ch/TC57/CIM100#RegulatingCondEq.RegulatingControl) | 0..1 <br />  [RegulatingControl](RegulatingControl.md)  | The regulating control scheme in which this equipment participates | [RegulatingCondEq](RegulatingCondEq.md) |
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
| self | cim:ShuntCompensator |
| native | this:ShuntCompensator |




