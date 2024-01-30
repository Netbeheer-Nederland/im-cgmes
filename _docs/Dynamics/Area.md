# Area


_Area._





**URI**: [cim:Area](http://iec.ch/TC57/CIM100#Area)<br />
**Type**: Class




```mermaid
 classDiagram
    class Area
      Area : Area.multiplier
        
          Area --> UnitMultiplier : Area.multiplier
        
      Area : Area.unit
        
          Area --> UnitSymbol : Area.unit
        
      Area : Area.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Area.value](http://iec.ch/TC57/CIM100#Area.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:Area.unit](http://iec.ch/TC57/CIM100#Area.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:Area.multiplier](http://iec.ch/TC57/CIM100#Area.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [GovHydroFrancis](GovHydroFrancis.md) | av0 | range | [Area](Area.md) |
| [GovHydroFrancis](GovHydroFrancis.md) | av1 | range | [Area](Area.md) |
| [GovHydroPelton](GovHydroPelton.md) | av0 | range | [Area](Area.md) |
| [GovHydroPelton](GovHydroPelton.md) | av1 | range | [Area](Area.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Area |
| native | this:Area |




