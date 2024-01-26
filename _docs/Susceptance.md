# Susceptance


_Imaginary part of admittance._





**URI**: [cim:Susceptance](http://iec.ch/TC57/CIM100#Susceptance)<br />
**Type**: Class




```mermaid
 classDiagram
    class Susceptance
      Susceptance : Susceptance.multiplier
        
          Susceptance --> UnitMultiplier : Susceptance.multiplier
        
      Susceptance : Susceptance.unit
        
          Susceptance --> UnitSymbol : Susceptance.unit
        
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
| [ACLineSegment](ACLineSegment.md) | bch | range | [Susceptance](Susceptance.md) |
| [EquivalentShunt](EquivalentShunt.md) | b | range | [Susceptance](Susceptance.md) |
| [LinearShuntCompensator](LinearShuntCompensator.md) | bPerSection | range | [Susceptance](Susceptance.md) |
| [NonlinearShuntCompensatorPoint](NonlinearShuntCompensatorPoint.md) | b | range | [Susceptance](Susceptance.md) |
| [PowerTransformerEnd](PowerTransformerEnd.md) | b | range | [Susceptance](Susceptance.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Susceptance |
| native | this:Susceptance |




