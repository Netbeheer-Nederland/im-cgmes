# StaticVarCompensator


_A facility for providing variable and controllable shunt reactive power. The SVC typically consists of a stepdown transformer, filter, thyristor-controlled reactor, and thyristor-switched capacitor arms._

__

_The SVC may operate in fixed MVar output mode or in voltage control mode. When in voltage control mode, the output of the SVC will be proportional to the deviation of voltage at the controlled bus from the voltage setpoint.  The SVC characteristic slope defines the proportion.  If the voltage at the controlled bus is equal to the voltage setpoint, the SVC MVar output is zero._





**URI**: [cim:StaticVarCompensator](http://iec.ch/TC57/CIM100#StaticVarCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class StaticVarCompensator
    click StaticVarCompensator href "../StaticVarCompensator"
      RegulatingCondEq <|-- StaticVarCompensator
        click RegulatingCondEq href "../RegulatingCondEq"
      
      StaticVarCompensator : Equipment.aggregate
        
      StaticVarCompensator : ConductingEquipment.BaseVoltage
        
          StaticVarCompensator --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      StaticVarCompensator : StaticVarCompensator.capacitiveRating
        
          StaticVarCompensator --> Reactance : StaticVarCompensator.capacitiveRating
          click Reactance href "../Reactance"
        
      StaticVarCompensator : IdentifiedObject.description
        
      StaticVarCompensator : IdentifiedObject.energyIdentCodeEic
        
      StaticVarCompensator : Equipment.EquipmentContainer
        
          StaticVarCompensator --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      StaticVarCompensator : StaticVarCompensator.inductiveRating
        
          StaticVarCompensator --> Reactance : StaticVarCompensator.inductiveRating
          click Reactance href "../Reactance"
        
      StaticVarCompensator : IdentifiedObject.mRID
        
      StaticVarCompensator : IdentifiedObject.name
        
      StaticVarCompensator : Equipment.normallyInService
        
      StaticVarCompensator : Equipment.OperationalLimitSet
        
          StaticVarCompensator --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      StaticVarCompensator : RegulatingCondEq.RegulatingControl
        
          StaticVarCompensator --> RegulatingControl : RegulatingCondEq.RegulatingControl
          click RegulatingControl href "../RegulatingControl"
        
      StaticVarCompensator : IdentifiedObject.shortName
        
      StaticVarCompensator : StaticVarCompensator.slope
        
          StaticVarCompensator --> VoltagePerReactivePower : StaticVarCompensator.slope
          click VoltagePerReactivePower href "../VoltagePerReactivePower"
        
      StaticVarCompensator : StaticVarCompensator.sVCControlMode
        
          StaticVarCompensator --> SVCControlMode : StaticVarCompensator.sVCControlMode
          click SVCControlMode href "../SVCControlMode"
        
      StaticVarCompensator : ConductingEquipment.Terminals
        
          StaticVarCompensator --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      StaticVarCompensator : StaticVarCompensator.voltageSetPoint
        
          StaticVarCompensator --> Voltage : StaticVarCompensator.voltageSetPoint
          click Voltage href "../Voltage"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * **StaticVarCompensator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| capacitiveRating | [cim:StaticVarCompensator.capacitiveRating](http://iec.ch/TC57/CIM100#StaticVarCompensator.capacitiveRating) | 1 <br />  [Reactance](Reactance.md)  | Capacitive reactance at maximum capacitive reactive power | direct |
| inductiveRating | [cim:StaticVarCompensator.inductiveRating](http://iec.ch/TC57/CIM100#StaticVarCompensator.inductiveRating) | 1 <br />  [Reactance](Reactance.md)  | Inductive reactance at maximum inductive reactive power | direct |
| slope | [cim:StaticVarCompensator.slope](http://iec.ch/TC57/CIM100#StaticVarCompensator.slope) | 1 <br />  [VoltagePerReactivePower](VoltagePerReactivePower.md)  | The characteristics slope of an SVC defines how the reactive power output cha... | direct |
| sVCControlMode | [cim:StaticVarCompensator.sVCControlMode](http://iec.ch/TC57/CIM100#StaticVarCompensator.sVCControlMode) | 0..1 <br />  [SVCControlMode](SVCControlMode.md)  | SVC control mode | direct |
| voltageSetPoint | [cim:StaticVarCompensator.voltageSetPoint](http://iec.ch/TC57/CIM100#StaticVarCompensator.voltageSetPoint) | 0..1 <br />  [Voltage](Voltage.md)  | The reactive power output of the SVC is proportional to the difference betwee... | direct |
| RegulatingControl | [cim:RegulatingCondEq.RegulatingControl](http://iec.ch/TC57/CIM100#RegulatingCondEq.RegulatingControl) | 0..1 <br />  [RegulatingControl](RegulatingControl.md)  | The regulating control scheme in which this equipment participates | [RegulatingCondEq](RegulatingCondEq.md) |
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









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:StaticVarCompensator |
| native | this:StaticVarCompensator |




