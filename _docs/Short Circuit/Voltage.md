# Voltage


_Electrical voltage, can be both AC and DC._





**URI**: [cim:Voltage](http://iec.ch/TC57/CIM100#Voltage)<br />
**Type**: Class




```mermaid
 classDiagram
    class Voltage
      Voltage : Voltage.multiplier
        
          Voltage --> UnitMultiplier : Voltage.multiplier
        
      Voltage : Voltage.unit
        
          Voltage --> UnitSymbol : Voltage.unit
        
      Voltage : Voltage.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:Voltage.value](http://iec.ch/TC57/CIM100#Voltage.value) | 0..1 <br />  float  |  | direct |
| multiplier | [cim:Voltage.multiplier](http://iec.ch/TC57/CIM100#Voltage.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:Voltage.unit](http://iec.ch/TC57/CIM100#Voltage.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [PetersenCoil](PetersenCoil.md) | nominalU | range | [Voltage](Voltage.md) |
| [PowerTransformer](PowerTransformer.md) | beforeShCircuitHighestOperatingVoltage | range | [Voltage](Voltage.md) |
| [PowerTransformer](PowerTransformer.md) | highSideMinOperatingU | range | [Voltage](Voltage.md) |
| [SeriesCompensator](SeriesCompensator.md) | varistorVoltageThreshold | range | [Voltage](Voltage.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Voltage |
| native | this:Voltage |




