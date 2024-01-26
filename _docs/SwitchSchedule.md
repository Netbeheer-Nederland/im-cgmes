# SwitchSchedule


_A schedule of switch positions.  If RegularTimePoint.value1 is 0, the switch is open.  If 1, the switch is closed._





**URI**: [cim:SwitchSchedule](http://iec.ch/TC57/CIM100#SwitchSchedule)<br />
**Type**: Class




```mermaid
 classDiagram
    class SwitchSchedule
      SeasonDayTypeSchedule <|-- SwitchSchedule
      
      SwitchSchedule : SeasonDayTypeSchedule.DayType
        
          SwitchSchedule --> DayType : SeasonDayTypeSchedule.DayType
        
      SwitchSchedule : IdentifiedObject.description
        
      SwitchSchedule : RegularIntervalSchedule.endTime
        
      SwitchSchedule : IdentifiedObject.energyIdentCodeEic
        
      SwitchSchedule : IdentifiedObject.mRID
        
      SwitchSchedule : IdentifiedObject.name
        
      SwitchSchedule : SeasonDayTypeSchedule.Season
        
          SwitchSchedule --> Season : SeasonDayTypeSchedule.Season
        
      SwitchSchedule : IdentifiedObject.shortName
        
      SwitchSchedule : BasicIntervalSchedule.startTime
        
      SwitchSchedule : SwitchSchedule.Switch
        
          SwitchSchedule --> Switch : SwitchSchedule.Switch
        
      SwitchSchedule : RegularIntervalSchedule.TimePoints
        
          SwitchSchedule --> RegularTimePoint : RegularIntervalSchedule.TimePoints
        
      SwitchSchedule : RegularIntervalSchedule.timeStep
        
          SwitchSchedule --> Seconds : RegularIntervalSchedule.timeStep
        
      SwitchSchedule : BasicIntervalSchedule.value1Unit
        
          SwitchSchedule --> UnitSymbol : BasicIntervalSchedule.value1Unit
        
      SwitchSchedule : BasicIntervalSchedule.value2Unit
        
          SwitchSchedule --> UnitSymbol : BasicIntervalSchedule.value2Unit
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [BasicIntervalSchedule](BasicIntervalSchedule.md)
        * [RegularIntervalSchedule](RegularIntervalSchedule.md)
            * [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md)
                * **SwitchSchedule**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Switch | [cim:SwitchSchedule.Switch](http://iec.ch/TC57/CIM100#SwitchSchedule.Switch) | 1..1 <br />  [Switch](Switch.md)  | A SwitchSchedule is associated with a Switch | direct |
| DayType | [cim:SeasonDayTypeSchedule.DayType](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule.DayType) | 1..1 <br />  [DayType](DayType.md)  | DayType for the Schedule | [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) |
| Season | [cim:SeasonDayTypeSchedule.Season](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule.Season) | 1..1 <br />  [Season](Season.md)  | Season for the Schedule | [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) |
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
| [Breaker](Breaker.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [Cut](Cut.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [Disconnector](Disconnector.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [DisconnectingCircuitBreaker](DisconnectingCircuitBreaker.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [Fuse](Fuse.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [GroundDisconnector](GroundDisconnector.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [Jumper](Jumper.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [LoadBreakSwitch](LoadBreakSwitch.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [ProtectedSwitch](ProtectedSwitch.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |
| [Switch](Switch.md) | SwitchSchedules | range | [SwitchSchedule](SwitchSchedule.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SwitchSchedule |
| native | this:SwitchSchedule |




