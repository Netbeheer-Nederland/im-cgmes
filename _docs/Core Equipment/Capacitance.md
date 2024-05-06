# Capacitance


_Capacitive part of reactance (imaginary part of impedance), at rated frequency._





**URI**: [cim:Capacitance](http://iec.ch/TC57/CIM100#Capacitance)<br />
**Type**: Class




```mermaid
 classDiagram
    class Capacitance
    click Capacitance href "../Capacitance"
      Capacitance : Capacitance.multiplier
        
          Capacitance --> UnitMultiplier : Capacitance.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Capacitance : Capacitance.unit
        
          Capacitance --> UnitSymbol : Capacitance.unit
          click UnitSymbol href "../UnitSymbol"
        
      Capacitance : Capacitance.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Capacitance.value](http://iec.ch/TC57/CIM100#Capacitance.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:Capacitance.unit](http://iec.ch/TC57/CIM100#Capacitance.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:Capacitance.multiplier](http://iec.ch/TC57/CIM100#Capacitance.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCLineSegment](DCLineSegment.md) | capacitance | range | [Capacitance](Capacitance.md) |
| [DCShunt](DCShunt.md) | capacitance | range | [Capacitance](Capacitance.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Capacitance |
| native | this:Capacitance |




