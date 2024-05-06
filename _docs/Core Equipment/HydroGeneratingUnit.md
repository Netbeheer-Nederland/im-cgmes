# HydroGeneratingUnit


_A generating unit whose prime mover is a hydraulic turbine (e.g., Francis, Pelton, Kaplan)._





**URI**: [cim:HydroGeneratingUnit](http://iec.ch/TC57/CIM100#HydroGeneratingUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class HydroGeneratingUnit
    click HydroGeneratingUnit href "../HydroGeneratingUnit"
      GeneratingUnit <|-- HydroGeneratingUnit
        click GeneratingUnit href "../GeneratingUnit"
      
      HydroGeneratingUnit : Equipment.aggregate
        
      HydroGeneratingUnit : GeneratingUnit.ControlAreaGeneratingUnit
        
          HydroGeneratingUnit --> ControlAreaGeneratingUnit : GeneratingUnit.ControlAreaGeneratingUnit
          click ControlAreaGeneratingUnit href "../ControlAreaGeneratingUnit"
        
      HydroGeneratingUnit : IdentifiedObject.description
        
      HydroGeneratingUnit : HydroGeneratingUnit.dropHeight
        
          HydroGeneratingUnit --> Length : HydroGeneratingUnit.dropHeight
          click Length href "../Length"
        
      HydroGeneratingUnit : HydroGeneratingUnit.energyConversionCapability
        
          HydroGeneratingUnit --> HydroEnergyConversionKind : HydroGeneratingUnit.energyConversionCapability
          click HydroEnergyConversionKind href "../HydroEnergyConversionKind"
        
      HydroGeneratingUnit : IdentifiedObject.energyIdentCodeEic
        
      HydroGeneratingUnit : Equipment.EquipmentContainer
        
          HydroGeneratingUnit --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      HydroGeneratingUnit : GeneratingUnit.genControlSource
        
          HydroGeneratingUnit --> GeneratorControlSource : GeneratingUnit.genControlSource
          click GeneratorControlSource href "../GeneratorControlSource"
        
      HydroGeneratingUnit : GeneratingUnit.governorSCD
        
          HydroGeneratingUnit --> PerCent : GeneratingUnit.governorSCD
          click PerCent href "../PerCent"
        
      HydroGeneratingUnit : GeneratingUnit.GrossToNetActivePowerCurves
        
          HydroGeneratingUnit --> GrossToNetActivePowerCurve : GeneratingUnit.GrossToNetActivePowerCurves
          click GrossToNetActivePowerCurve href "../GrossToNetActivePowerCurve"
        
      HydroGeneratingUnit : HydroGeneratingUnit.HydroPowerPlant
        
          HydroGeneratingUnit --> HydroPowerPlant : HydroGeneratingUnit.HydroPowerPlant
          click HydroPowerPlant href "../HydroPowerPlant"
        
      HydroGeneratingUnit : GeneratingUnit.longPF
        
      HydroGeneratingUnit : GeneratingUnit.maximumAllowableSpinningReserve
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.maximumAllowableSpinningReserve
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : GeneratingUnit.maxOperatingP
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.maxOperatingP
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : GeneratingUnit.minOperatingP
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.minOperatingP
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : IdentifiedObject.mRID
        
      HydroGeneratingUnit : IdentifiedObject.name
        
      HydroGeneratingUnit : GeneratingUnit.nominalP
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.nominalP
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : Equipment.normallyInService
        
      HydroGeneratingUnit : Equipment.OperationalLimitSet
        
          HydroGeneratingUnit --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      HydroGeneratingUnit : GeneratingUnit.ratedGrossMaxP
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.ratedGrossMaxP
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : GeneratingUnit.ratedGrossMinP
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.ratedGrossMinP
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : GeneratingUnit.ratedNetMaxP
        
          HydroGeneratingUnit --> ActivePower : GeneratingUnit.ratedNetMaxP
          click ActivePower href "../ActivePower"
        
      HydroGeneratingUnit : GeneratingUnit.RotatingMachine
        
          HydroGeneratingUnit --> RotatingMachine : GeneratingUnit.RotatingMachine
          click RotatingMachine href "../RotatingMachine"
        
      HydroGeneratingUnit : IdentifiedObject.shortName
        
      HydroGeneratingUnit : GeneratingUnit.shortPF
        
      HydroGeneratingUnit : GeneratingUnit.startupCost
        
          HydroGeneratingUnit --> Money : GeneratingUnit.startupCost
          click Money href "../Money"
        
      HydroGeneratingUnit : GeneratingUnit.startupTime
        
          HydroGeneratingUnit --> Seconds : GeneratingUnit.startupTime
          click Seconds href "../Seconds"
        
      HydroGeneratingUnit : GeneratingUnit.totalEfficiency
        
          HydroGeneratingUnit --> PerCent : GeneratingUnit.totalEfficiency
          click PerCent href "../PerCent"
        
      HydroGeneratingUnit : HydroGeneratingUnit.turbineType
        
          HydroGeneratingUnit --> HydroTurbineKind : HydroGeneratingUnit.turbineType
          click HydroTurbineKind href "../HydroTurbineKind"
        
      HydroGeneratingUnit : GeneratingUnit.variableCost
        
          HydroGeneratingUnit --> Money : GeneratingUnit.variableCost
          click Money href "../Money"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
                * **HydroGeneratingUnit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| energyConversionCapability | [cim:HydroGeneratingUnit.energyConversionCapability](http://iec.ch/TC57/CIM100#HydroGeneratingUnit.energyConversionCapability) | 0..1 <br />  [HydroEnergyConversionKind](HydroEnergyConversionKind.md)  | Energy conversion capability for generating | direct |
| dropHeight | [cim:HydroGeneratingUnit.dropHeight](http://iec.ch/TC57/CIM100#HydroGeneratingUnit.dropHeight) | 0..1 <br />  [Length](Length.md)  | The height water drops from the reservoir mid-point to the turbine | direct |
| turbineType | [cim:HydroGeneratingUnit.turbineType](http://iec.ch/TC57/CIM100#HydroGeneratingUnit.turbineType) | 0..1 <br />  [HydroTurbineKind](HydroTurbineKind.md)  | Type of turbine | direct |
| HydroPowerPlant | [cim:HydroGeneratingUnit.HydroPowerPlant](http://iec.ch/TC57/CIM100#HydroGeneratingUnit.HydroPowerPlant) | 0..1 <br />  [HydroPowerPlant](HydroPowerPlant.md)  | The hydro generating unit belongs to a hydro power plant | direct |
| ControlAreaGeneratingUnit | [cim:GeneratingUnit.ControlAreaGeneratingUnit](http://iec.ch/TC57/CIM100#GeneratingUnit.ControlAreaGeneratingUnit) | * <br />  [ControlAreaGeneratingUnit](ControlAreaGeneratingUnit.md)  | ControlArea specifications for this generating unit | [GeneratingUnit](GeneratingUnit.md) |
| genControlSource | [cim:GeneratingUnit.genControlSource](http://iec.ch/TC57/CIM100#GeneratingUnit.genControlSource) | 0..1 <br />  [GeneratorControlSource](GeneratorControlSource.md)  | The source of controls for a generating unit | [GeneratingUnit](GeneratingUnit.md) |
| governorSCD | [cim:GeneratingUnit.governorSCD](http://iec.ch/TC57/CIM100#GeneratingUnit.governorSCD) | 0..1 <br />  [PerCent](PerCent.md)  | Governor Speed Changer Droop | [GeneratingUnit](GeneratingUnit.md) |
| longPF | [cim:GeneratingUnit.longPF](http://iec.ch/TC57/CIM100#GeneratingUnit.longPF) | 0..1 <br />  float  | Generating unit long term economic participation factor | [GeneratingUnit](GeneratingUnit.md) |
| maximumAllowableSpinningReserve | [cim:GeneratingUnit.maximumAllowableSpinningReserve](http://iec.ch/TC57/CIM100#GeneratingUnit.maximumAllowableSpinningReserve) | 0..1 <br />  [ActivePower](ActivePower.md)  | Maximum allowable spinning reserve | [GeneratingUnit](GeneratingUnit.md) |
| maxOperatingP | [cim:GeneratingUnit.maxOperatingP](http://iec.ch/TC57/CIM100#GeneratingUnit.maxOperatingP) | 1 <br />  [ActivePower](ActivePower.md)  | This is the maximum operating active power limit the dispatcher can enter for... | [GeneratingUnit](GeneratingUnit.md) |
| minOperatingP | [cim:GeneratingUnit.minOperatingP](http://iec.ch/TC57/CIM100#GeneratingUnit.minOperatingP) | 1 <br />  [ActivePower](ActivePower.md)  | This is the minimum operating active power limit the dispatcher can enter for... | [GeneratingUnit](GeneratingUnit.md) |
| nominalP | [cim:GeneratingUnit.nominalP](http://iec.ch/TC57/CIM100#GeneratingUnit.nominalP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The nominal power of the generating unit | [GeneratingUnit](GeneratingUnit.md) |
| ratedGrossMaxP | [cim:GeneratingUnit.ratedGrossMaxP](http://iec.ch/TC57/CIM100#GeneratingUnit.ratedGrossMaxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The unit's gross rated maximum capacity (book value) | [GeneratingUnit](GeneratingUnit.md) |
| ratedGrossMinP | [cim:GeneratingUnit.ratedGrossMinP](http://iec.ch/TC57/CIM100#GeneratingUnit.ratedGrossMinP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The gross rated minimum generation level which the unit can safely operate at... | [GeneratingUnit](GeneratingUnit.md) |
| ratedNetMaxP | [cim:GeneratingUnit.ratedNetMaxP](http://iec.ch/TC57/CIM100#GeneratingUnit.ratedNetMaxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The net rated maximum capacity determined by subtracting the auxiliary power ... | [GeneratingUnit](GeneratingUnit.md) |
| shortPF | [cim:GeneratingUnit.shortPF](http://iec.ch/TC57/CIM100#GeneratingUnit.shortPF) | 0..1 <br />  float  | Generating unit short term economic participation factor | [GeneratingUnit](GeneratingUnit.md) |
| startupCost | [cim:GeneratingUnit.startupCost](http://iec.ch/TC57/CIM100#GeneratingUnit.startupCost) | 0..1 <br />  [Money](Money.md)  | The initial startup cost incurred for each start of the GeneratingUnit | [GeneratingUnit](GeneratingUnit.md) |
| variableCost | [cim:GeneratingUnit.variableCost](http://iec.ch/TC57/CIM100#GeneratingUnit.variableCost) | 0..1 <br />  [Money](Money.md)  | The variable cost component of production per unit of ActivePower | [GeneratingUnit](GeneratingUnit.md) |
| startupTime | [cim:GeneratingUnit.startupTime](http://iec.ch/TC57/CIM100#GeneratingUnit.startupTime) | 0..1 <br />  [Seconds](Seconds.md)  | Time it takes to get the unit on-line, from the time that the prime mover mec... | [GeneratingUnit](GeneratingUnit.md) |
| totalEfficiency | [cim:GeneratingUnit.totalEfficiency](http://iec.ch/TC57/CIM100#GeneratingUnit.totalEfficiency) | 0..1 <br />  [PerCent](PerCent.md)  | The efficiency of the unit in converting the fuel into electrical energy | [GeneratingUnit](GeneratingUnit.md) |
| GrossToNetActivePowerCurves | [cim:GeneratingUnit.GrossToNetActivePowerCurves](http://iec.ch/TC57/CIM100#GeneratingUnit.GrossToNetActivePowerCurves) | * <br />  [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md)  | A generating unit may have a gross active power to net active power curve, de... | [GeneratingUnit](GeneratingUnit.md) |
| RotatingMachine | [cim:GeneratingUnit.RotatingMachine](http://iec.ch/TC57/CIM100#GeneratingUnit.RotatingMachine) | 1..* <br />  [RotatingMachine](RotatingMachine.md)  | A synchronous machine may operate as a generator and as such becomes a member... | [GeneratingUnit](GeneratingUnit.md) |
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
| [HydroPowerPlant](HydroPowerPlant.md) | HydroGeneratingUnits | range | [HydroGeneratingUnit](HydroGeneratingUnit.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:HydroGeneratingUnit |
| native | this:HydroGeneratingUnit |




