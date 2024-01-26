# RegularIntervalSchedule


_The schedule has time points where the time between them is constant._





**URI**: [cim:RegularIntervalSchedule](http://iec.ch/TC57/CIM100#RegularIntervalSchedule)<br />
**Type**: Class




```mermaid
 classDiagram
    class RegularIntervalSchedule
      BasicIntervalSchedule <|-- RegularIntervalSchedule
      

      RegularIntervalSchedule <|-- SeasonDayTypeSchedule
      
      
      RegularIntervalSchedule : IdentifiedObject.description
        
      RegularIntervalSchedule : RegularIntervalSchedule.endTime
        
      RegularIntervalSchedule : IdentifiedObject.energyIdentCodeEic
        
      RegularIntervalSchedule : IdentifiedObject.mRID
        
      RegularIntervalSchedule : IdentifiedObject.name
        
      RegularIntervalSchedule : IdentifiedObject.shortName
        
      RegularIntervalSchedule : BasicIntervalSchedule.startTime
        
      RegularIntervalSchedule : RegularIntervalSchedule.TimePoints
        
          RegularIntervalSchedule --> RegularTimePoint : RegularIntervalSchedule.TimePoints
        
      RegularIntervalSchedule : RegularIntervalSchedule.timeStep
        
          RegularIntervalSchedule --> Seconds : RegularIntervalSchedule.timeStep
        
      RegularIntervalSchedule : BasicIntervalSchedule.value1Unit
        
          RegularIntervalSchedule --> UnitSymbol : BasicIntervalSchedule.value1Unit
        
      RegularIntervalSchedule : BasicIntervalSchedule.value2Unit
        
          RegularIntervalSchedule --> UnitSymbol : BasicIntervalSchedule.value2Unit
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [BasicIntervalSchedule](BasicIntervalSchedule.md)
        * **RegularIntervalSchedule**
            * [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| TimePoints | [cim:RegularIntervalSchedule.TimePoints](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.TimePoints) | 1..* <br />  [RegularTimePoint](RegularTimePoint.md)  | The regular interval time point data values that define this schedule | direct |
| timeStep | [cim:RegularIntervalSchedule.timeStep](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.timeStep) | 1..1 <br />  [Seconds](Seconds.md)  | The time between each pair of subsequent regular time points in sequence orde... | direct |
| endTime | [cim:RegularIntervalSchedule.endTime](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.endTime) | 1..1 <br />  date  | The time for the last time point | direct |
| startTime | [cim:BasicIntervalSchedule.startTime](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.startTime) | 1..1 <br />  date  | The time for the first time point | [BasicIntervalSchedule](BasicIntervalSchedule.md) |
| value1Unit | [cim:BasicIntervalSchedule.value1Unit](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.value1Unit) | 1..1 <br />  [UnitSymbol](UnitSymbol.md)  | Value1 units of measure | [BasicIntervalSchedule](BasicIntervalSchedule.md) |
| value2Unit | [cim:BasicIntervalSchedule.value2Unit](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.value2Unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | Value2 units of measure | [BasicIntervalSchedule](BasicIntervalSchedule.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RegularTimePoint](RegularTimePoint.md) | IntervalSchedule | range | [RegularIntervalSchedule](RegularIntervalSchedule.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RegularIntervalSchedule |
| native | this:RegularIntervalSchedule |




