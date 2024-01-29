# SynchronousMachine


_An electromechanical device that operates with shaft rotating synchronously with the network. It is a single machine operating either as a generator or synchronous condenser or pump._





**URI**: [cim:SynchronousMachine](http://iec.ch/TC57/CIM100#SynchronousMachine)<br />
**Type**: Class




```mermaid
 classDiagram
    class SynchronousMachine
      RotatingMachine <|-- SynchronousMachine
      
      SynchronousMachine : Equipment.aggregate
        
      SynchronousMachine : ConductingEquipment.BaseVoltage
        
          SynchronousMachine --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      SynchronousMachine : IdentifiedObject.description
        
      SynchronousMachine : IdentifiedObject.energyIdentCodeEic
        
      SynchronousMachine : Equipment.EquipmentContainer
        
          SynchronousMachine --> EquipmentContainer : Equipment.EquipmentContainer
        
      SynchronousMachine : RotatingMachine.GeneratingUnit
        
          SynchronousMachine --> GeneratingUnit : RotatingMachine.GeneratingUnit
        
      SynchronousMachine : RotatingMachine.HydroPump
        
          SynchronousMachine --> HydroPump : RotatingMachine.HydroPump
        
      SynchronousMachine : SynchronousMachine.InitialReactiveCapabilityCurve
        
          SynchronousMachine --> ReactiveCapabilityCurve : SynchronousMachine.InitialReactiveCapabilityCurve
        
      SynchronousMachine : SynchronousMachine.maxQ
        
          SynchronousMachine --> ReactivePower : SynchronousMachine.maxQ
        
      SynchronousMachine : SynchronousMachine.minQ
        
          SynchronousMachine --> ReactivePower : SynchronousMachine.minQ
        
      SynchronousMachine : IdentifiedObject.mRID
        
      SynchronousMachine : IdentifiedObject.name
        
      SynchronousMachine : Equipment.normallyInService
        
      SynchronousMachine : Equipment.OperationalLimitSet
        
          SynchronousMachine --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      SynchronousMachine : SynchronousMachine.qPercent
        
          SynchronousMachine --> PerCent : SynchronousMachine.qPercent
        
      SynchronousMachine : RotatingMachine.ratedPowerFactor
        
      SynchronousMachine : RotatingMachine.ratedS
        
          SynchronousMachine --> ApparentPower : RotatingMachine.ratedS
        
      SynchronousMachine : RotatingMachine.ratedU
        
          SynchronousMachine --> Voltage : RotatingMachine.ratedU
        
      SynchronousMachine : RegulatingCondEq.RegulatingControl
        
          SynchronousMachine --> RegulatingControl : RegulatingCondEq.RegulatingControl
        
      SynchronousMachine : IdentifiedObject.shortName
        
      SynchronousMachine : ConductingEquipment.Terminals
        
          SynchronousMachine --> Terminal : ConductingEquipment.Terminals
        
      SynchronousMachine : SynchronousMachine.type
        
          SynchronousMachine --> SynchronousMachineKind : SynchronousMachine.type
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * [RotatingMachine](RotatingMachine.md)
                            * **SynchronousMachine**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| InitialReactiveCapabilityCurve | [cim:SynchronousMachine.InitialReactiveCapabilityCurve](http://iec.ch/TC57/CIM100#SynchronousMachine.InitialReactiveCapabilityCurve) | 0..1 <br />  [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md)  | The default reactive capability curve for use by a synchronous machine | direct |
| maxQ | [cim:SynchronousMachine.maxQ](http://iec.ch/TC57/CIM100#SynchronousMachine.maxQ) | 0..1 <br />  [ReactivePower](ReactivePower.md)  | Maximum reactive power limit | direct |
| minQ | [cim:SynchronousMachine.minQ](http://iec.ch/TC57/CIM100#SynchronousMachine.minQ) | 0..1 <br />  [ReactivePower](ReactivePower.md)  | Minimum reactive power limit for the unit | direct |
| qPercent | [cim:SynchronousMachine.qPercent](http://iec.ch/TC57/CIM100#SynchronousMachine.qPercent) | 0..1 <br />  [PerCent](PerCent.md)  | Part of the coordinated reactive control that comes from this machine | direct |
| type | [cim:SynchronousMachine.type](http://iec.ch/TC57/CIM100#SynchronousMachine.type) | 1..1 <br />  [SynchronousMachineKind](SynchronousMachineKind.md)  | Modes that this synchronous machine can operate in | direct |
| GeneratingUnit | [cim:RotatingMachine.GeneratingUnit](http://iec.ch/TC57/CIM100#RotatingMachine.GeneratingUnit) | 0..1 <br />  [GeneratingUnit](GeneratingUnit.md)  | A synchronous machine may operate as a generator and as such becomes a member... | [RotatingMachine](RotatingMachine.md) |
| HydroPump | [cim:RotatingMachine.HydroPump](http://iec.ch/TC57/CIM100#RotatingMachine.HydroPump) | 0..1 <br />  [HydroPump](HydroPump.md)  | The synchronous machine drives the turbine which moves the water from a low e... | [RotatingMachine](RotatingMachine.md) |
| ratedPowerFactor | [cim:RotatingMachine.ratedPowerFactor](http://iec.ch/TC57/CIM100#RotatingMachine.ratedPowerFactor) | 0..1 <br />  float  | Power factor (nameplate data) | [RotatingMachine](RotatingMachine.md) |
| ratedS | [cim:RotatingMachine.ratedS](http://iec.ch/TC57/CIM100#RotatingMachine.ratedS) | 0..1 <br />  [ApparentPower](ApparentPower.md)  | Nameplate apparent power rating for the unit | [RotatingMachine](RotatingMachine.md) |
| ratedU | [cim:RotatingMachine.ratedU](http://iec.ch/TC57/CIM100#RotatingMachine.ratedU) | 0..1 <br />  [Voltage](Voltage.md)  | Rated voltage (nameplate data, Ur in IEC 60909-0) | [RotatingMachine](RotatingMachine.md) |
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





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md) | InitiallyUsedBySynchronousMachines | range | [SynchronousMachine](SynchronousMachine.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SynchronousMachine |
| native | this:SynchronousMachine |




