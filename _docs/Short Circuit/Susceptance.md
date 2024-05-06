# Susceptance


_Imaginary part of admittance._





**URI**: [cim:Susceptance](http://iec.ch/TC57/CIM100#Susceptance)<br />
**Type**: Class




```mermaid
 classDiagram
    class Susceptance
    click Susceptance href "../Susceptance"
      Susceptance : Susceptance.multiplier
        
          Susceptance --> UnitMultiplier : Susceptance.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Susceptance : Susceptance.unit
        
          Susceptance --> UnitSymbol : Susceptance.unit
          click UnitSymbol href "../UnitSymbol"
        
      Susceptance : Susceptance.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Susceptance.value](http://iec.ch/TC57/CIM100#Susceptance.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:Susceptance.unit](http://iec.ch/TC57/CIM100#Susceptance.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:Susceptance.multiplier](http://iec.ch/TC57/CIM100#Susceptance.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACLineSegment](ACLineSegment.md) | b0ch | range | [Susceptance](Susceptance.md) |
| [LinearShuntCompensator](LinearShuntCompensator.md) | b0PerSection | range | [Susceptance](Susceptance.md) |
| [MutualCoupling](MutualCoupling.md) | b0ch | range | [Susceptance](Susceptance.md) |
| [NonlinearShuntCompensatorPoint](NonlinearShuntCompensatorPoint.md) | b0 | range | [Susceptance](Susceptance.md) |
| [PowerTransformerEnd](PowerTransformerEnd.md) | b0 | range | [Susceptance](Susceptance.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Susceptance |
| native | this:Susceptance |




