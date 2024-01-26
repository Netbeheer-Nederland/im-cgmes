# RotationSpeed


_Number of revolutions per second._





**URI**: [cim:RotationSpeed](http://iec.ch/TC57/CIM100#RotationSpeed)<br />
**Type**: Class




```mermaid
 classDiagram
    class RotationSpeed
      RotationSpeed : RotationSpeed.multiplier
        
          RotationSpeed --> UnitMultiplier : RotationSpeed.multiplier
        
      RotationSpeed : RotationSpeed.unit
        
          RotationSpeed --> UnitSymbol : RotationSpeed.unit
        
      RotationSpeed : RotationSpeed.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| multiplier | [cim:RotationSpeed.multiplier](http://iec.ch/TC57/CIM100#RotationSpeed.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:RotationSpeed.unit](http://iec.ch/TC57/CIM100#RotationSpeed.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| value | [cim:RotationSpeed.value](http://iec.ch/TC57/CIM100#RotationSpeed.value) | 0..1 <br />  float  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [AsynchronousMachine](AsynchronousMachine.md) | nominalSpeed | range | [RotationSpeed](RotationSpeed.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RotationSpeed |
| native | this:RotationSpeed |




