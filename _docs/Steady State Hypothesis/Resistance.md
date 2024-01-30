# Resistance


_Resistance (real part of impedance)._





**URI**: [cim:Resistance](http://iec.ch/TC57/CIM100#Resistance)<br />
**Type**: Class




```mermaid
 classDiagram
    class Resistance
      Resistance : Resistance.multiplier
        
          Resistance --> UnitMultiplier : Resistance.multiplier
        
      Resistance : Resistance.unit
        
          Resistance --> UnitSymbol : Resistance.unit
        
      Resistance : Resistance.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Resistance.value](http://iec.ch/TC57/CIM100#Resistance.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:Resistance.unit](http://iec.ch/TC57/CIM100#Resistance.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:Resistance.multiplier](http://iec.ch/TC57/CIM100#Resistance.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [VsConverter](VsConverter.md) | droopCompensation | range | [Resistance](Resistance.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Resistance |
| native | this:Resistance |




