# WindGeneratingUnit


_A wind driven generating unit, connected to the grid by means of a rotating machine.  May be used to represent a single turbine or an aggregation._





**URI**: [cim:WindGeneratingUnit](http://iec.ch/TC57/CIM100#WindGeneratingUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindGeneratingUnit
      GeneratingUnit <|-- WindGeneratingUnit
      
      WindGeneratingUnit : Equipment.aggregate
        
      WindGeneratingUnit : GeneratingUnit.ControlAreaGeneratingUnit
        
          WindGeneratingUnit --> ControlAreaGeneratingUnit : GeneratingUnit.ControlAreaGeneratingUnit
        
      WindGeneratingUnit : IdentifiedObject.description
        
      WindGeneratingUnit : IdentifiedObject.energyIdentCodeEic
        
      WindGeneratingUnit : Equipment.EquipmentContainer
        
          WindGeneratingUnit --> EquipmentContainer : Equipment.EquipmentContainer
        
      WindGeneratingUnit : GeneratingUnit.genControlSource
        
          WindGeneratingUnit --> GeneratorControlSource : GeneratingUnit.genControlSource
        
      WindGeneratingUnit : GeneratingUnit.governorSCD
        
          WindGeneratingUnit --> PerCent : GeneratingUnit.governorSCD
        
      WindGeneratingUnit : GeneratingUnit.GrossToNetActivePowerCurves
        
          WindGeneratingUnit --> GrossToNetActivePowerCurve : GeneratingUnit.GrossToNetActivePowerCurves
        
      WindGeneratingUnit : GeneratingUnit.longPF
        
      WindGeneratingUnit : GeneratingUnit.maximumAllowableSpinningReserve
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.maximumAllowableSpinningReserve
        
      WindGeneratingUnit : GeneratingUnit.maxOperatingP
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.maxOperatingP
        
      WindGeneratingUnit : GeneratingUnit.minOperatingP
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.minOperatingP
        
      WindGeneratingUnit : IdentifiedObject.mRID
        
      WindGeneratingUnit : IdentifiedObject.name
        
      WindGeneratingUnit : GeneratingUnit.nominalP
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.nominalP
        
      WindGeneratingUnit : Equipment.normallyInService
        
      WindGeneratingUnit : Equipment.OperationalLimitSet
        
          WindGeneratingUnit --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      WindGeneratingUnit : GeneratingUnit.ratedGrossMaxP
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.ratedGrossMaxP
        
      WindGeneratingUnit : GeneratingUnit.ratedGrossMinP
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.ratedGrossMinP
        
      WindGeneratingUnit : GeneratingUnit.ratedNetMaxP
        
          WindGeneratingUnit --> ActivePower : GeneratingUnit.ratedNetMaxP
        
      WindGeneratingUnit : GeneratingUnit.RotatingMachine
        
          WindGeneratingUnit --> RotatingMachine : GeneratingUnit.RotatingMachine
        
      WindGeneratingUnit : IdentifiedObject.shortName
        
      WindGeneratingUnit : GeneratingUnit.shortPF
        
      WindGeneratingUnit : GeneratingUnit.startupCost
        
          WindGeneratingUnit --> Money : GeneratingUnit.startupCost
        
      WindGeneratingUnit : GeneratingUnit.startupTime
        
          WindGeneratingUnit --> Seconds : GeneratingUnit.startupTime
        
      WindGeneratingUnit : GeneratingUnit.totalEfficiency
        
          WindGeneratingUnit --> PerCent : GeneratingUnit.totalEfficiency
        
      WindGeneratingUnit : GeneratingUnit.variableCost
        
          WindGeneratingUnit --> Money : GeneratingUnit.variableCost
        
      WindGeneratingUnit : WindGeneratingUnit.windGenUnitType
        
          WindGeneratingUnit --> WindGenUnitKind : WindGeneratingUnit.windGenUnitType
        
      WindGeneratingUnit : WindGeneratingUnit.WindPowerPlant
        
          WindGeneratingUnit --> WindPowerPlant : WindGeneratingUnit.WindPowerPlant
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
                * **WindGeneratingUnit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| windGenUnitType | [cim:WindGeneratingUnit.windGenUnitType](http://iec.ch/TC57/CIM100#WindGeneratingUnit.windGenUnitType) | 1..1 <br />  [WindGenUnitKind](WindGenUnitKind.md)  | The kind of wind generating unit | direct |
| WindPowerPlant | [eu:WindGeneratingUnit.WindPowerPlant](http://iec.ch/TC57/CIM100-European#WindGeneratingUnit.WindPowerPlant) | 0..1 <br />  [WindPowerPlant](WindPowerPlant.md)  | A wind power plant may have wind generating units | direct |
| ControlAreaGeneratingUnit | [cim:GeneratingUnit.ControlAreaGeneratingUnit](http://iec.ch/TC57/CIM100#GeneratingUnit.ControlAreaGeneratingUnit) | 0..* <br />  [ControlAreaGeneratingUnit](ControlAreaGeneratingUnit.md)  | ControlArea specifications for this generating unit | [GeneratingUnit](GeneratingUnit.md) |
| genControlSource | [cim:GeneratingUnit.genControlSource](http://iec.ch/TC57/CIM100#GeneratingUnit.genControlSource) | 0..1 <br />  [GeneratorControlSource](GeneratorControlSource.md)  | The source of controls for a generating unit | [GeneratingUnit](GeneratingUnit.md) |
| governorSCD | [cim:GeneratingUnit.governorSCD](http://iec.ch/TC57/CIM100#GeneratingUnit.governorSCD) | 0..1 <br />  [PerCent](PerCent.md)  | Governor Speed Changer Droop | [GeneratingUnit](GeneratingUnit.md) |
| longPF | [cim:GeneratingUnit.longPF](http://iec.ch/TC57/CIM100#GeneratingUnit.longPF) | 0..1 <br />  float  | Generating unit long term economic participation factor | [GeneratingUnit](GeneratingUnit.md) |
| maximumAllowableSpinningReserve | [cim:GeneratingUnit.maximumAllowableSpinningReserve](http://iec.ch/TC57/CIM100#GeneratingUnit.maximumAllowableSpinningReserve) | 0..1 <br />  [ActivePower](ActivePower.md)  | Maximum allowable spinning reserve | [GeneratingUnit](GeneratingUnit.md) |
| maxOperatingP | [cim:GeneratingUnit.maxOperatingP](http://iec.ch/TC57/CIM100#GeneratingUnit.maxOperatingP) | 1..1 <br />  [ActivePower](ActivePower.md)  | This is the maximum operating active power limit the dispatcher can enter for... | [GeneratingUnit](GeneratingUnit.md) |
| minOperatingP | [cim:GeneratingUnit.minOperatingP](http://iec.ch/TC57/CIM100#GeneratingUnit.minOperatingP) | 1..1 <br />  [ActivePower](ActivePower.md)  | This is the minimum operating active power limit the dispatcher can enter for... | [GeneratingUnit](GeneratingUnit.md) |
| nominalP | [cim:GeneratingUnit.nominalP](http://iec.ch/TC57/CIM100#GeneratingUnit.nominalP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The nominal power of the generating unit | [GeneratingUnit](GeneratingUnit.md) |
| ratedGrossMaxP | [cim:GeneratingUnit.ratedGrossMaxP](http://iec.ch/TC57/CIM100#GeneratingUnit.ratedGrossMaxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The unit's gross rated maximum capacity (book value) | [GeneratingUnit](GeneratingUnit.md) |
| ratedGrossMinP | [cim:GeneratingUnit.ratedGrossMinP](http://iec.ch/TC57/CIM100#GeneratingUnit.ratedGrossMinP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The gross rated minimum generation level which the unit can safely operate at... | [GeneratingUnit](GeneratingUnit.md) |
| ratedNetMaxP | [cim:GeneratingUnit.ratedNetMaxP](http://iec.ch/TC57/CIM100#GeneratingUnit.ratedNetMaxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | The net rated maximum capacity determined by subtracting the auxiliary power ... | [GeneratingUnit](GeneratingUnit.md) |
| shortPF | [cim:GeneratingUnit.shortPF](http://iec.ch/TC57/CIM100#GeneratingUnit.shortPF) | 0..1 <br />  float  | Generating unit short term economic participation factor | [GeneratingUnit](GeneratingUnit.md) |
| startupCost | [cim:GeneratingUnit.startupCost](http://iec.ch/TC57/CIM100#GeneratingUnit.startupCost) | 0..1 <br />  [Money](Money.md)  | The initial startup cost incurred for each start of the GeneratingUnit | [GeneratingUnit](GeneratingUnit.md) |
| variableCost | [cim:GeneratingUnit.variableCost](http://iec.ch/TC57/CIM100#GeneratingUnit.variableCost) | 0..1 <br />  [Money](Money.md)  | The variable cost component of production per unit of ActivePower | [GeneratingUnit](GeneratingUnit.md) |
| startupTime | [cim:GeneratingUnit.startupTime](http://iec.ch/TC57/CIM100#GeneratingUnit.startupTime) | 0..1 <br />  [Seconds](Seconds.md)  | Time it takes to get the unit on-line, from the time that the prime mover mec... | [GeneratingUnit](GeneratingUnit.md) |
| totalEfficiency | [cim:GeneratingUnit.totalEfficiency](http://iec.ch/TC57/CIM100#GeneratingUnit.totalEfficiency) | 0..1 <br />  [PerCent](PerCent.md)  | The efficiency of the unit in converting the fuel into electrical energy | [GeneratingUnit](GeneratingUnit.md) |
| GrossToNetActivePowerCurves | [cim:GeneratingUnit.GrossToNetActivePowerCurves](http://iec.ch/TC57/CIM100#GeneratingUnit.GrossToNetActivePowerCurves) | 0..* <br />  [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md)  | A generating unit may have a gross active power to net active power curve, de... | [GeneratingUnit](GeneratingUnit.md) |
| RotatingMachine | [cim:GeneratingUnit.RotatingMachine](http://iec.ch/TC57/CIM100#GeneratingUnit.RotatingMachine) | 1..* <br />  [RotatingMachine](RotatingMachine.md)  | A synchronous machine may operate as a generator and as such becomes a member... | [GeneratingUnit](GeneratingUnit.md) |
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
| [WindPowerPlant](WindPowerPlant.md) | WindGeneratingUnits | range | [WindGeneratingUnit](WindGeneratingUnit.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindGeneratingUnit |
| native | this:WindGeneratingUnit |




