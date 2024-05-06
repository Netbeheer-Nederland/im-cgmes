# LinearShuntCompensator


_A linear shunt compensator has banks or sections with equal admittance values._





**URI**: [cim:LinearShuntCompensator](http://iec.ch/TC57/CIM100#LinearShuntCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class LinearShuntCompensator
    click LinearShuntCompensator href "../LinearShuntCompensator"
      ShuntCompensator <|-- LinearShuntCompensator
        click ShuntCompensator href "../ShuntCompensator"
      
      LinearShuntCompensator : Equipment.aggregate
        
      LinearShuntCompensator : ShuntCompensator.aVRDelay
        
          LinearShuntCompensator --> Seconds : ShuntCompensator.aVRDelay
          click Seconds href "../Seconds"
        
      LinearShuntCompensator : ConductingEquipment.BaseVoltage
        
          LinearShuntCompensator --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      LinearShuntCompensator : LinearShuntCompensator.bPerSection
        
          LinearShuntCompensator --> Susceptance : LinearShuntCompensator.bPerSection
          click Susceptance href "../Susceptance"
        
      LinearShuntCompensator : IdentifiedObject.description
        
      LinearShuntCompensator : IdentifiedObject.energyIdentCodeEic
        
      LinearShuntCompensator : Equipment.EquipmentContainer
        
          LinearShuntCompensator --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      LinearShuntCompensator : LinearShuntCompensator.gPerSection
        
          LinearShuntCompensator --> Conductance : LinearShuntCompensator.gPerSection
          click Conductance href "../Conductance"
        
      LinearShuntCompensator : ShuntCompensator.grounded
        
      LinearShuntCompensator : ShuntCompensator.maximumSections
        
      LinearShuntCompensator : IdentifiedObject.mRID
        
      LinearShuntCompensator : IdentifiedObject.name
        
      LinearShuntCompensator : ShuntCompensator.nomU
        
          LinearShuntCompensator --> Voltage : ShuntCompensator.nomU
          click Voltage href "../Voltage"
        
      LinearShuntCompensator : Equipment.normallyInService
        
      LinearShuntCompensator : ShuntCompensator.normalSections
        
      LinearShuntCompensator : Equipment.OperationalLimitSet
        
          LinearShuntCompensator --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      LinearShuntCompensator : RegulatingCondEq.RegulatingControl
        
          LinearShuntCompensator --> RegulatingControl : RegulatingCondEq.RegulatingControl
          click RegulatingControl href "../RegulatingControl"
        
      LinearShuntCompensator : IdentifiedObject.shortName
        
      LinearShuntCompensator : ConductingEquipment.Terminals
        
          LinearShuntCompensator --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      LinearShuntCompensator : ShuntCompensator.voltageSensitivity
        
          LinearShuntCompensator --> VoltagePerReactivePower : ShuntCompensator.voltageSensitivity
          click VoltagePerReactivePower href "../VoltagePerReactivePower"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * [ShuntCompensator](ShuntCompensator.md)
                            * **LinearShuntCompensator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| bPerSection | [cim:LinearShuntCompensator.bPerSection](http://iec.ch/TC57/CIM100#LinearShuntCompensator.bPerSection) | 1 <br />  [Susceptance](Susceptance.md)  | Positive sequence shunt (charging) susceptance per section | direct |
| gPerSection | [cim:LinearShuntCompensator.gPerSection](http://iec.ch/TC57/CIM100#LinearShuntCompensator.gPerSection) | 1 <br />  [Conductance](Conductance.md)  | Positive sequence shunt (charging) conductance per section | direct |
| aVRDelay | [cim:ShuntCompensator.aVRDelay](http://iec.ch/TC57/CIM100#ShuntCompensator.aVRDelay) | 0..1 <br />  [Seconds](Seconds.md)  | An automatic voltage regulation delay (AVRDelay) which is the time delay from... | [ShuntCompensator](ShuntCompensator.md) |
| grounded | [cim:ShuntCompensator.grounded](http://iec.ch/TC57/CIM100#ShuntCompensator.grounded) | 0..1 <br />  boolean  | Used for Yn and Zn connections | [ShuntCompensator](ShuntCompensator.md) |
| maximumSections | [cim:ShuntCompensator.maximumSections](http://iec.ch/TC57/CIM100#ShuntCompensator.maximumSections) | 1 <br />  integer  | The maximum number of sections that may be switched in | [ShuntCompensator](ShuntCompensator.md) |
| nomU | [cim:ShuntCompensator.nomU](http://iec.ch/TC57/CIM100#ShuntCompensator.nomU) | 1 <br />  [Voltage](Voltage.md)  | The voltage at which the nominal reactive power may be calculated | [ShuntCompensator](ShuntCompensator.md) |
| normalSections | [cim:ShuntCompensator.normalSections](http://iec.ch/TC57/CIM100#ShuntCompensator.normalSections) | 1 <br />  integer  | The normal number of sections switched in | [ShuntCompensator](ShuntCompensator.md) |
| voltageSensitivity | [cim:ShuntCompensator.voltageSensitivity](http://iec.ch/TC57/CIM100#ShuntCompensator.voltageSensitivity) | 0..1 <br />  [VoltagePerReactivePower](VoltagePerReactivePower.md)  | Voltage sensitivity required for the device to regulate the bus voltage, in v... | [ShuntCompensator](ShuntCompensator.md) |
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
| self | cim:LinearShuntCompensator |
| native | this:LinearShuntCompensator |




