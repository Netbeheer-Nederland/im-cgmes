# PerCent


_Percentage on a defined base.   For example, specify as 100 to indicate at the defined base._





**URI**: [cim:PerCent](http://iec.ch/TC57/CIM100#PerCent)<br />
**Type**: Class




```mermaid
 classDiagram
    class PerCent
    click PerCent href "../PerCent"
      PerCent : PerCent.multiplier
        
          PerCent --> UnitMultiplier : PerCent.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      PerCent : PerCent.unit
        
          PerCent --> UnitSymbol : PerCent.unit
          click UnitSymbol href "../UnitSymbol"
        
      PerCent : PerCent.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:PerCent.value](http://iec.ch/TC57/CIM100#PerCent.value) | 0..1 <br />  float  | Normally 0 to 100 on a defined base | direct |
| unit | [cim:PerCent.unit](http://iec.ch/TC57/CIM100#PerCent.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:PerCent.multiplier](http://iec.ch/TC57/CIM100#PerCent.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConformLoad](ConformLoad.md) | pfixedPct | range | [PerCent](PerCent.md) |
| [ConformLoad](ConformLoad.md) | qfixedPct | range | [PerCent](PerCent.md) |
| [EnergyConsumer](EnergyConsumer.md) | pfixedPct | range | [PerCent](PerCent.md) |
| [EnergyConsumer](EnergyConsumer.md) | qfixedPct | range | [PerCent](PerCent.md) |
| [GeneratingUnit](GeneratingUnit.md) | governorSCD | range | [PerCent](PerCent.md) |
| [GeneratingUnit](GeneratingUnit.md) | totalEfficiency | range | [PerCent](PerCent.md) |
| [HydroGeneratingUnit](HydroGeneratingUnit.md) | governorSCD | range | [PerCent](PerCent.md) |
| [HydroGeneratingUnit](HydroGeneratingUnit.md) | totalEfficiency | range | [PerCent](PerCent.md) |
| [NonConformLoad](NonConformLoad.md) | pfixedPct | range | [PerCent](PerCent.md) |
| [NonConformLoad](NonConformLoad.md) | qfixedPct | range | [PerCent](PerCent.md) |
| [NuclearGeneratingUnit](NuclearGeneratingUnit.md) | governorSCD | range | [PerCent](PerCent.md) |
| [NuclearGeneratingUnit](NuclearGeneratingUnit.md) | totalEfficiency | range | [PerCent](PerCent.md) |
| [PhaseTapChangerAsymmetrical](PhaseTapChangerAsymmetrical.md) | voltageStepIncrement | range | [PerCent](PerCent.md) |
| [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md) | voltageStepIncrement | range | [PerCent](PerCent.md) |
| [PhaseTapChangerSymmetrical](PhaseTapChangerSymmetrical.md) | voltageStepIncrement | range | [PerCent](PerCent.md) |
| [PhaseTapChangerTablePoint](PhaseTapChangerTablePoint.md) | b | range | [PerCent](PerCent.md) |
| [PhaseTapChangerTablePoint](PhaseTapChangerTablePoint.md) | g | range | [PerCent](PerCent.md) |
| [PhaseTapChangerTablePoint](PhaseTapChangerTablePoint.md) | r | range | [PerCent](PerCent.md) |
| [PhaseTapChangerTablePoint](PhaseTapChangerTablePoint.md) | x | range | [PerCent](PerCent.md) |
| [RatioTapChanger](RatioTapChanger.md) | stepVoltageIncrement | range | [PerCent](PerCent.md) |
| [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md) | b | range | [PerCent](PerCent.md) |
| [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md) | g | range | [PerCent](PerCent.md) |
| [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md) | r | range | [PerCent](PerCent.md) |
| [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md) | x | range | [PerCent](PerCent.md) |
| [SolarGeneratingUnit](SolarGeneratingUnit.md) | governorSCD | range | [PerCent](PerCent.md) |
| [SolarGeneratingUnit](SolarGeneratingUnit.md) | totalEfficiency | range | [PerCent](PerCent.md) |
| [StationSupply](StationSupply.md) | pfixedPct | range | [PerCent](PerCent.md) |
| [StationSupply](StationSupply.md) | qfixedPct | range | [PerCent](PerCent.md) |
| [SynchronousMachine](SynchronousMachine.md) | qPercent | range | [PerCent](PerCent.md) |
| [TapChangerTablePoint](TapChangerTablePoint.md) | b | range | [PerCent](PerCent.md) |
| [TapChangerTablePoint](TapChangerTablePoint.md) | g | range | [PerCent](PerCent.md) |
| [TapChangerTablePoint](TapChangerTablePoint.md) | r | range | [PerCent](PerCent.md) |
| [TapChangerTablePoint](TapChangerTablePoint.md) | x | range | [PerCent](PerCent.md) |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | governorSCD | range | [PerCent](PerCent.md) |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | totalEfficiency | range | [PerCent](PerCent.md) |
| [WindGeneratingUnit](WindGeneratingUnit.md) | governorSCD | range | [PerCent](PerCent.md) |
| [WindGeneratingUnit](WindGeneratingUnit.md) | totalEfficiency | range | [PerCent](PerCent.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PerCent |
| native | this:PerCent |




