# Inductance


_Inductive part of reactance (imaginary part of impedance), at rated frequency._





**URI**: [cim:Inductance](http://iec.ch/TC57/CIM100#Inductance)<br />
**Type**: Class




```mermaid
 classDiagram
    class Inductance
    click Inductance href "../Inductance"
      Inductance : Inductance.multiplier
        
          Inductance --> UnitMultiplier : Inductance.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Inductance : Inductance.unit
        
          Inductance --> UnitSymbol : Inductance.unit
          click UnitSymbol href "../UnitSymbol"
        
      Inductance : Inductance.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Inductance.value](http://iec.ch/TC57/CIM100#Inductance.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:Inductance.unit](http://iec.ch/TC57/CIM100#Inductance.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:Inductance.multiplier](http://iec.ch/TC57/CIM100#Inductance.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCGround](DCGround.md) | inductance | range | [Inductance](Inductance.md) |
| [DCLineSegment](DCLineSegment.md) | inductance | range | [Inductance](Inductance.md) |
| [DCSeriesDevice](DCSeriesDevice.md) | inductance | range | [Inductance](Inductance.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Inductance |
| native | this:Inductance |




