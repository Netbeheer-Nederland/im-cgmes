# AngleRadians


_Phase angle in radians._





**URI**: [cim:AngleRadians](http://iec.ch/TC57/CIM100#AngleRadians)<br />
**Type**: Class




```mermaid
 classDiagram
    class AngleRadians
    click AngleRadians href "../AngleRadians"
      AngleRadians : AngleRadians.multiplier
        
          AngleRadians --> UnitMultiplier : AngleRadians.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      AngleRadians : AngleRadians.unit
        
          AngleRadians --> UnitSymbol : AngleRadians.unit
          click UnitSymbol href "../UnitSymbol"
        
      AngleRadians : AngleRadians.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:AngleRadians.value](http://iec.ch/TC57/CIM100#AngleRadians.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:AngleRadians.unit](http://iec.ch/TC57/CIM100#AngleRadians.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:AngleRadians.multiplier](http://iec.ch/TC57/CIM100#AngleRadians.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [EnergySource](EnergySource.md) | voltageAngle | range | [AngleRadians](AngleRadians.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AngleRadians |
| native | this:AngleRadians |




