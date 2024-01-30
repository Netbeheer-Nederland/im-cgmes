# SeriesCompensator


_A Series Compensator is a series capacitor or reactor or an AC transmission line without charging susceptance.  It is a two terminal device._





**URI**: [cim:SeriesCompensator](http://iec.ch/TC57/CIM100#SeriesCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class SeriesCompensator
      ConductingEquipment <|-- SeriesCompensator
      
      SeriesCompensator : IdentifiedObject.mRID
        
      SeriesCompensator : SeriesCompensator.r0
        
          SeriesCompensator --> Resistance : SeriesCompensator.r0
        
      SeriesCompensator : SeriesCompensator.varistorPresent
        
      SeriesCompensator : SeriesCompensator.varistorRatedCurrent
        
          SeriesCompensator --> CurrentFlow : SeriesCompensator.varistorRatedCurrent
        
      SeriesCompensator : SeriesCompensator.varistorVoltageThreshold
        
          SeriesCompensator --> Voltage : SeriesCompensator.varistorVoltageThreshold
        
      SeriesCompensator : SeriesCompensator.x0
        
          SeriesCompensator --> Reactance : SeriesCompensator.x0
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **SeriesCompensator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| r0 | [cim:SeriesCompensator.r0](http://iec.ch/TC57/CIM100#SeriesCompensator.r0) | 1..1 <br />  [Resistance](Resistance.md)  | Zero sequence resistance | direct |
| x0 | [cim:SeriesCompensator.x0](http://iec.ch/TC57/CIM100#SeriesCompensator.x0) | 1..1 <br />  [Reactance](Reactance.md)  | Zero sequence reactance | direct |
| varistorPresent | [cim:SeriesCompensator.varistorPresent](http://iec.ch/TC57/CIM100#SeriesCompensator.varistorPresent) | 1..1 <br />  boolean  | Describe if a metal oxide varistor (mov) for over voltage protection is confi... | direct |
| varistorRatedCurrent | [cim:SeriesCompensator.varistorRatedCurrent](http://iec.ch/TC57/CIM100#SeriesCompensator.varistorRatedCurrent) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The maximum current the varistor is designed to handle at specified duration | direct |
| varistorVoltageThreshold | [cim:SeriesCompensator.varistorVoltageThreshold](http://iec.ch/TC57/CIM100#SeriesCompensator.varistorVoltageThreshold) | 0..1 <br />  [Voltage](Voltage.md)  | The dc voltage at which the varistor starts conducting | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SeriesCompensator |
| native | this:SeriesCompensator |




