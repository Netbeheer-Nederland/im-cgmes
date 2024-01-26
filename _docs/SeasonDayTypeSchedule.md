# SeasonDayTypeSchedule


_A time schedule covering a 24 hour period, with curve data for a specific type of season and day._





**URI**: [cim:SeasonDayTypeSchedule](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule)<br />
**Type**: Class




```mermaid
 classDiagram
    class SeasonDayTypeSchedule
      RegularIntervalSchedule <|-- SeasonDayTypeSchedule
      

      SeasonDayTypeSchedule <|-- ConformLoadSchedule
      SeasonDayTypeSchedule <|-- RegulationSchedule
      SeasonDayTypeSchedule <|-- TapSchedule
      SeasonDayTypeSchedule <|-- NonConformLoadSchedule
      SeasonDayTypeSchedule <|-- SwitchSchedule
      
      
      SeasonDayTypeSchedule : SeasonDayTypeSchedule.DayType
        
          SeasonDayTypeSchedule --> DayType : SeasonDayTypeSchedule.DayType
        
      SeasonDayTypeSchedule : IdentifiedObject.description
        
      SeasonDayTypeSchedule : RegularIntervalSchedule.endTime
        
      SeasonDayTypeSchedule : IdentifiedObject.energyIdentCodeEic
        
      SeasonDayTypeSchedule : IdentifiedObject.mRID
        
      SeasonDayTypeSchedule : IdentifiedObject.name
        
      SeasonDayTypeSchedule : SeasonDayTypeSchedule.Season
        
          SeasonDayTypeSchedule --> Season : SeasonDayTypeSchedule.Season
        
      SeasonDayTypeSchedule : IdentifiedObject.shortName
        
      SeasonDayTypeSchedule : BasicIntervalSchedule.startTime
        
      SeasonDayTypeSchedule : RegularIntervalSchedule.TimePoints
        
          SeasonDayTypeSchedule --> RegularTimePoint : RegularIntervalSchedule.TimePoints
        
      SeasonDayTypeSchedule : RegularIntervalSchedule.timeStep
        
          SeasonDayTypeSchedule --> Seconds : RegularIntervalSchedule.timeStep
        
      SeasonDayTypeSchedule : BasicIntervalSchedule.value1Unit
        
          SeasonDayTypeSchedule --> UnitSymbol : BasicIntervalSchedule.value1Unit
        
      SeasonDayTypeSchedule : BasicIntervalSchedule.value2Unit
        
          SeasonDayTypeSchedule --> UnitSymbol : BasicIntervalSchedule.value2Unit
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [BasicIntervalSchedule](BasicIntervalSchedule.md)
        * [RegularIntervalSchedule](RegularIntervalSchedule.md)
            * **SeasonDayTypeSchedule**
                * [ConformLoadSchedule](ConformLoadSchedule.md)
                * [RegulationSchedule](RegulationSchedule.md)
                * [TapSchedule](TapSchedule.md)
                * [NonConformLoadSchedule](NonConformLoadSchedule.md)
                * [SwitchSchedule](SwitchSchedule.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DayType | [cim:SeasonDayTypeSchedule.DayType](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule.DayType) | 1..1 <br />  [DayType](DayType.md)  | DayType for the Schedule | direct |
| Season | [cim:SeasonDayTypeSchedule.Season](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule.Season) | 1..1 <br />  [Season](Season.md)  | Season for the Schedule | direct |
| TimePoints | [cim:RegularIntervalSchedule.TimePoints](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.TimePoints) | 1..* <br />  [RegularTimePoint](RegularTimePoint.md)  | The regular interval time point data values that define this schedule | [RegularIntervalSchedule](RegularIntervalSchedule.md) |
| timeStep | [cim:RegularIntervalSchedule.timeStep](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.timeStep) | 1..1 <br />  [Seconds](Seconds.md)  | The time between each pair of subsequent regular time points in sequence orde... | [RegularIntervalSchedule](RegularIntervalSchedule.md) |
| endTime | [cim:RegularIntervalSchedule.endTime](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.endTime) | 1..1 <br />  date  | The time for the last time point | [RegularIntervalSchedule](RegularIntervalSchedule.md) |
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
| [DayType](DayType.md) | SeasonDayTypeSchedules | range | [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) |
| [Season](Season.md) | SeasonDayTypeSchedules | range | [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SeasonDayTypeSchedule |
| native | this:SeasonDayTypeSchedule |




