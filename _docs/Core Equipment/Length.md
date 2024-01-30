# Length


_Unit of length. It shall be a positive value or zero._





**URI**: [cim:Length](http://iec.ch/TC57/CIM100#Length)<br />
**Type**: Class




```mermaid
 classDiagram
    class Length
      Length : Length.multiplier
        
          Length --> UnitMultiplier : Length.multiplier
        
      Length : Length.unit
        
          Length --> UnitSymbol : Length.unit
        
      Length : Length.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Length.value](http://iec.ch/TC57/CIM100#Length.value) | 0..1 <br />  float  |  | direct |
| unit | [cim:Length.unit](http://iec.ch/TC57/CIM100#Length.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| multiplier | [cim:Length.multiplier](http://iec.ch/TC57/CIM100#Length.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACLineSegment](ACLineSegment.md) | length | range | [Length](Length.md) |
| [Clamp](Clamp.md) | lengthFromTerminal1 | range | [Length](Length.md) |
| [Conductor](Conductor.md) | length | range | [Length](Length.md) |
| [Cut](Cut.md) | lengthFromTerminal1 | range | [Length](Length.md) |
| [DCLineSegment](DCLineSegment.md) | length | range | [Length](Length.md) |
| [HydroGeneratingUnit](HydroGeneratingUnit.md) | dropHeight | range | [Length](Length.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Length |
| native | this:Length |




