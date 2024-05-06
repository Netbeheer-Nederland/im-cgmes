# ActivePowerPerCurrentFlow


_Active power variation with current flow._





**URI**: [cim:ActivePowerPerCurrentFlow](http://iec.ch/TC57/CIM100#ActivePowerPerCurrentFlow)<br />
**Type**: Class




```mermaid
 classDiagram
    class ActivePowerPerCurrentFlow
    click ActivePowerPerCurrentFlow href "../ActivePowerPerCurrentFlow"
      ActivePowerPerCurrentFlow : ActivePowerPerCurrentFlow.multiplier
        
          ActivePowerPerCurrentFlow --> UnitMultiplier : ActivePowerPerCurrentFlow.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      ActivePowerPerCurrentFlow : ActivePowerPerCurrentFlow.unit
        
          ActivePowerPerCurrentFlow --> UnitSymbol : ActivePowerPerCurrentFlow.unit
          click UnitSymbol href "../UnitSymbol"
        
      ActivePowerPerCurrentFlow : ActivePowerPerCurrentFlow.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| multiplier | [cim:ActivePowerPerCurrentFlow.multiplier](http://iec.ch/TC57/CIM100#ActivePowerPerCurrentFlow.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:ActivePowerPerCurrentFlow.unit](http://iec.ch/TC57/CIM100#ActivePowerPerCurrentFlow.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| value | [cim:ActivePowerPerCurrentFlow.value](http://iec.ch/TC57/CIM100#ActivePowerPerCurrentFlow.value) | 0..1 <br />  float  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACDCConverter](ACDCConverter.md) | switchingLoss | range | [ActivePowerPerCurrentFlow](ActivePowerPerCurrentFlow.md) |
| [CsConverter](CsConverter.md) | switchingLoss | range | [ActivePowerPerCurrentFlow](ActivePowerPerCurrentFlow.md) |
| [VsConverter](VsConverter.md) | switchingLoss | range | [ActivePowerPerCurrentFlow](ActivePowerPerCurrentFlow.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ActivePowerPerCurrentFlow |
| native | this:ActivePowerPerCurrentFlow |




