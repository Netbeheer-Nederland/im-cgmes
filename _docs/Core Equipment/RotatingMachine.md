# RotatingMachine


_A rotating machine which may be used as a generator or motor._





**URI**: [cim:RotatingMachine](http://iec.ch/TC57/CIM100#RotatingMachine)<br />
**Type**: Class




```mermaid
 classDiagram
    class RotatingMachine
    click RotatingMachine href "../RotatingMachine"
      RegulatingCondEq <|-- RotatingMachine
        click RegulatingCondEq href "../RegulatingCondEq"
      

      RotatingMachine <|-- AsynchronousMachine
        click AsynchronousMachine href "../AsynchronousMachine"
      RotatingMachine <|-- SynchronousMachine
        click SynchronousMachine href "../SynchronousMachine"
      
      
      RotatingMachine : Equipment.aggregate
        
      RotatingMachine : ConductingEquipment.BaseVoltage
        
          RotatingMachine --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      RotatingMachine : IdentifiedObject.description
        
      RotatingMachine : IdentifiedObject.energyIdentCodeEic
        
      RotatingMachine : Equipment.EquipmentContainer
        
          RotatingMachine --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      RotatingMachine : RotatingMachine.GeneratingUnit
        
          RotatingMachine --> GeneratingUnit : RotatingMachine.GeneratingUnit
          click GeneratingUnit href "../GeneratingUnit"
        
      RotatingMachine : RotatingMachine.HydroPump
        
          RotatingMachine --> HydroPump : RotatingMachine.HydroPump
          click HydroPump href "../HydroPump"
        
      RotatingMachine : IdentifiedObject.mRID
        
      RotatingMachine : IdentifiedObject.name
        
      RotatingMachine : Equipment.normallyInService
        
      RotatingMachine : Equipment.OperationalLimitSet
        
          RotatingMachine --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      RotatingMachine : RotatingMachine.ratedPowerFactor
        
      RotatingMachine : RotatingMachine.ratedS
        
          RotatingMachine --> ApparentPower : RotatingMachine.ratedS
          click ApparentPower href "../ApparentPower"
        
      RotatingMachine : RotatingMachine.ratedU
        
          RotatingMachine --> Voltage : RotatingMachine.ratedU
          click Voltage href "../Voltage"
        
      RotatingMachine : RegulatingCondEq.RegulatingControl
        
          RotatingMachine --> RegulatingControl : RegulatingCondEq.RegulatingControl
          click RegulatingControl href "../RegulatingControl"
        
      RotatingMachine : IdentifiedObject.shortName
        
      RotatingMachine : ConductingEquipment.Terminals
        
          RotatingMachine --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * **RotatingMachine**
                            * [AsynchronousMachine](AsynchronousMachine.md)
                            * [SynchronousMachine](SynchronousMachine.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| GeneratingUnit | [cim:RotatingMachine.GeneratingUnit](http://iec.ch/TC57/CIM100#RotatingMachine.GeneratingUnit) | 0..1 <br />  [GeneratingUnit](GeneratingUnit.md)  | A synchronous machine may operate as a generator and as such becomes a member... | direct |
| HydroPump | [cim:RotatingMachine.HydroPump](http://iec.ch/TC57/CIM100#RotatingMachine.HydroPump) | 0..1 <br />  [HydroPump](HydroPump.md)  | The synchronous machine drives the turbine which moves the water from a low e... | direct |
| ratedPowerFactor | [cim:RotatingMachine.ratedPowerFactor](http://iec.ch/TC57/CIM100#RotatingMachine.ratedPowerFactor) | 0..1 <br />  float  | Power factor (nameplate data) | direct |
| ratedS | [cim:RotatingMachine.ratedS](http://iec.ch/TC57/CIM100#RotatingMachine.ratedS) | 0..1 <br />  [ApparentPower](ApparentPower.md)  | Nameplate apparent power rating for the unit | direct |
| ratedU | [cim:RotatingMachine.ratedU](http://iec.ch/TC57/CIM100#RotatingMachine.ratedU) | 0..1 <br />  [Voltage](Voltage.md)  | Rated voltage (nameplate data, Ur in IEC 60909-0) | direct |
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





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [GeneratingUnit](GeneratingUnit.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |
| [HydroGeneratingUnit](HydroGeneratingUnit.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |
| [HydroPump](HydroPump.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |
| [NuclearGeneratingUnit](NuclearGeneratingUnit.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |
| [SolarGeneratingUnit](SolarGeneratingUnit.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |
| [WindGeneratingUnit](WindGeneratingUnit.md) | RotatingMachine | range | [RotatingMachine](RotatingMachine.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RotatingMachine |
| native | this:RotatingMachine |




