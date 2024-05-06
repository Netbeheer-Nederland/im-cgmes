# Temperature


_Value of temperature in degrees Celsius._





**URI**: [cim:Temperature](http://iec.ch/TC57/CIM100#Temperature)<br />
**Type**: Class




```mermaid
 classDiagram
    class Temperature
    click Temperature href "../Temperature"
      Temperature : Temperature.multiplier
        
          Temperature --> UnitMultiplier : Temperature.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Temperature : Temperature.unit
        
          Temperature --> UnitSymbol : Temperature.unit
          click UnitSymbol href "../UnitSymbol"
        
      Temperature : Temperature.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| multiplier | [cim:Temperature.multiplier](http://iec.ch/TC57/CIM100#Temperature.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:Temperature.unit](http://iec.ch/TC57/CIM100#Temperature.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| value | [cim:Temperature.value](http://iec.ch/TC57/CIM100#Temperature.value) | 0..1 <br />  float  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACLineSegment](ACLineSegment.md) | shortCircuitEndTemperature | range | [Temperature](Temperature.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Temperature |
| native | this:Temperature |




