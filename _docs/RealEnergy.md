# RealEnergy


_Real electrical energy._





**URI**: [cim:RealEnergy](http://iec.ch/TC57/CIM100#RealEnergy)<br />
**Type**: Class




```mermaid
 classDiagram
    class RealEnergy
      RealEnergy : RealEnergy.multiplier
        
          RealEnergy --> UnitMultiplier : RealEnergy.multiplier
        
      RealEnergy : RealEnergy.unit
        
          RealEnergy --> UnitSymbol : RealEnergy.unit
        
      RealEnergy : RealEnergy.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| multiplier | [cim:RealEnergy.multiplier](http://iec.ch/TC57/CIM100#RealEnergy.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:RealEnergy.unit](http://iec.ch/TC57/CIM100#RealEnergy.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| value | [cim:RealEnergy.value](http://iec.ch/TC57/CIM100#RealEnergy.value) | 0..1 <br />  float  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [BatteryUnit](BatteryUnit.md) | ratedE | range | [RealEnergy](RealEnergy.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RealEnergy |
| native | this:RealEnergy |




