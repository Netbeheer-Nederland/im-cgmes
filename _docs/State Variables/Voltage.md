# Voltage


_Electrical voltage, can be both AC and DC._





**URI**: [cim:Voltage](http://iec.ch/TC57/CIM100#Voltage)<br />
**Type**: Class




```mermaid
 classDiagram
    class Voltage
    click Voltage href "../Voltage"
      Voltage : Voltage.multiplier
        
          Voltage --> UnitMultiplier : Voltage.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Voltage : Voltage.unit
        
          Voltage --> UnitSymbol : Voltage.unit
          click UnitSymbol href "../UnitSymbol"
        
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
| [ACDCConverter](ACDCConverter.md) | uc | range | [Voltage](Voltage.md) |
| [ACDCConverter](ACDCConverter.md) | udc | range | [Voltage](Voltage.md) |
| [CsConverter](CsConverter.md) | uc | range | [Voltage](Voltage.md) |
| [CsConverter](CsConverter.md) | udc | range | [Voltage](Voltage.md) |
| [SvVoltage](SvVoltage.md) | v | range | [Voltage](Voltage.md) |
| [VsConverter](VsConverter.md) | uv | range | [Voltage](Voltage.md) |
| [VsConverter](VsConverter.md) | uc | range | [Voltage](Voltage.md) |
| [VsConverter](VsConverter.md) | udc | range | [Voltage](Voltage.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/StateVariables-EU#Package_StateVariablesProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Voltage |
| native | this:Voltage |




