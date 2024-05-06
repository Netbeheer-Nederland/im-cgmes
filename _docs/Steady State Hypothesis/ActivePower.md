# ActivePower


_Product of RMS value of the voltage and the RMS value of the in-phase component of the current._





**URI**: [cim:ActivePower](http://iec.ch/TC57/CIM100#ActivePower)<br />
**Type**: Class




```mermaid
 classDiagram
    class ActivePower
    click ActivePower href "../ActivePower"
      ActivePower : ActivePower.multiplier
        
          ActivePower --> UnitMultiplier : ActivePower.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      ActivePower : ActivePower.unit
        
          ActivePower --> UnitSymbol : ActivePower.unit
          click UnitSymbol href "../UnitSymbol"
        
      ActivePower : ActivePower.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:ActivePower.value](http://iec.ch/TC57/CIM100#ActivePower.value) | 0..1 <br />  float  |  | direct |
| multiplier | [cim:ActivePower.multiplier](http://iec.ch/TC57/CIM100#ActivePower.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:ActivePower.unit](http://iec.ch/TC57/CIM100#ActivePower.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACDCConverter](ACDCConverter.md) | p | range | [ActivePower](ActivePower.md) |
| [ACDCConverter](ACDCConverter.md) | targetPpcc | range | [ActivePower](ActivePower.md) |
| [ActivePowerLimit](ActivePowerLimit.md) | value | range | [ActivePower](ActivePower.md) |
| [AsynchronousMachine](AsynchronousMachine.md) | p | range | [ActivePower](ActivePower.md) |
| [ConformLoad](ConformLoad.md) | p | range | [ActivePower](ActivePower.md) |
| [ControlArea](ControlArea.md) | netInterchange | range | [ActivePower](ActivePower.md) |
| [ControlArea](ControlArea.md) | pTolerance | range | [ActivePower](ActivePower.md) |
| [CsConverter](CsConverter.md) | p | range | [ActivePower](ActivePower.md) |
| [CsConverter](CsConverter.md) | targetPpcc | range | [ActivePower](ActivePower.md) |
| [EnergyConsumer](EnergyConsumer.md) | p | range | [ActivePower](ActivePower.md) |
| [EnergySource](EnergySource.md) | activePower | range | [ActivePower](ActivePower.md) |
| [EquivalentInjection](EquivalentInjection.md) | p | range | [ActivePower](ActivePower.md) |
| [ExternalNetworkInjection](ExternalNetworkInjection.md) | p | range | [ActivePower](ActivePower.md) |
| [NonConformLoad](NonConformLoad.md) | p | range | [ActivePower](ActivePower.md) |
| [PowerElectronicsConnection](PowerElectronicsConnection.md) | p | range | [ActivePower](ActivePower.md) |
| [RotatingMachine](RotatingMachine.md) | p | range | [ActivePower](ActivePower.md) |
| [StationSupply](StationSupply.md) | p | range | [ActivePower](ActivePower.md) |
| [SynchronousMachine](SynchronousMachine.md) | p | range | [ActivePower](ActivePower.md) |
| [VsConverter](VsConverter.md) | p | range | [ActivePower](ActivePower.md) |
| [VsConverter](VsConverter.md) | targetPpcc | range | [ActivePower](ActivePower.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ActivePower |
| native | this:ActivePower |




