# ActivePowerPerFrequency


_Active power variation with frequency._





**URI**: [cim:ActivePowerPerFrequency](http://iec.ch/TC57/CIM100#ActivePowerPerFrequency)<br />
**Type**: Class




```mermaid
 classDiagram
    class ActivePowerPerFrequency
    click ActivePowerPerFrequency href "../ActivePowerPerFrequency"
      ActivePowerPerFrequency : ActivePowerPerFrequency.multiplier
        
          ActivePowerPerFrequency --> UnitMultiplier : ActivePowerPerFrequency.multiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      ActivePowerPerFrequency : ActivePowerPerFrequency.unit
        
          ActivePowerPerFrequency --> UnitSymbol : ActivePowerPerFrequency.unit
          click UnitSymbol href "../UnitSymbol"
        
      ActivePowerPerFrequency : ActivePowerPerFrequency.value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| multiplier | [cim:ActivePowerPerFrequency.multiplier](http://iec.ch/TC57/CIM100#ActivePowerPerFrequency.multiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  |  | direct |
| unit | [cim:ActivePowerPerFrequency.unit](http://iec.ch/TC57/CIM100#ActivePowerPerFrequency.unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  |  | direct |
| value | [cim:ActivePowerPerFrequency.value](http://iec.ch/TC57/CIM100#ActivePowerPerFrequency.value) | 0..1 <br />  float  |  | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ExternalNetworkInjection](ExternalNetworkInjection.md) | governorSCD | range | [ActivePowerPerFrequency](ActivePowerPerFrequency.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ActivePowerPerFrequency |
| native | this:ActivePowerPerFrequency |




