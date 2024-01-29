# AngleDegrees


_Measurement of angle in degrees._





**URI**: [cim:AngleDegrees](http://iec.ch/TC57/CIM100#AngleDegrees)<br />
**Type**: Class




```mermaid
 classDiagram
    class AngleDegrees
      AngleDegrees : AngleDegrees.multiplier
        
          AngleDegrees --> UnitMultiplier : AngleDegrees.multiplier
        
      AngleDegrees : AngleDegrees.unit
        
          AngleDegrees --> UnitSymbol : AngleDegrees.unit
        
      AngleDegrees : AngleDegrees.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:AngleDegrees.value](http://iec.ch/TC57/CIM100#AngleDegrees.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:AngleDegrees.unit](http://iec.ch/TC57/CIM100#AngleDegrees.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:AngleDegrees.multiplier](http://iec.ch/TC57/CIM100#AngleDegrees.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DiagramObject](DiagramObject.md) | rotation | range | [AngleDegrees](AngleDegrees.md) |
| [TextDiagramObject](TextDiagramObject.md) | rotation | range | [AngleDegrees](AngleDegrees.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/DiagramLayout-EU#Package_DiagramLayoutProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AngleDegrees |
| native | this:AngleDegrees |




