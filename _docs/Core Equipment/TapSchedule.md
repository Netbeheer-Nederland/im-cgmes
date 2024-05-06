# TapSchedule


_A pre-established pattern over time for a tap step._





**URI**: [cim:TapSchedule](http://iec.ch/TC57/CIM100#TapSchedule)<br />
**Type**: Class




```mermaid
 classDiagram
    class TapSchedule
    click TapSchedule href "../TapSchedule"
      SeasonDayTypeSchedule <|-- TapSchedule
        click SeasonDayTypeSchedule href "../SeasonDayTypeSchedule"
      
      TapSchedule : SeasonDayTypeSchedule.DayType
        
          TapSchedule --> DayType : SeasonDayTypeSchedule.DayType
          click DayType href "../DayType"
        
      TapSchedule : IdentifiedObject.description
        
      TapSchedule : RegularIntervalSchedule.endTime
        
      TapSchedule : IdentifiedObject.energyIdentCodeEic
        
      TapSchedule : IdentifiedObject.mRID
        
      TapSchedule : IdentifiedObject.name
        
      TapSchedule : SeasonDayTypeSchedule.Season
        
          TapSchedule --> Season : SeasonDayTypeSchedule.Season
          click Season href "../Season"
        
      TapSchedule : IdentifiedObject.shortName
        
      TapSchedule : BasicIntervalSchedule.startTime
        
      TapSchedule : TapSchedule.TapChanger
        
          TapSchedule --> TapChanger : TapSchedule.TapChanger
          click TapChanger href "../TapChanger"
        
      TapSchedule : RegularIntervalSchedule.TimePoints
        
          TapSchedule --> RegularTimePoint : RegularIntervalSchedule.TimePoints
          click RegularTimePoint href "../RegularTimePoint"
        
      TapSchedule : RegularIntervalSchedule.timeStep
        
          TapSchedule --> Seconds : RegularIntervalSchedule.timeStep
          click Seconds href "../Seconds"
        
      TapSchedule : BasicIntervalSchedule.value1Unit
        
          TapSchedule --> UnitSymbol : BasicIntervalSchedule.value1Unit
          click UnitSymbol href "../UnitSymbol"
        
      TapSchedule : BasicIntervalSchedule.value2Unit
        
          TapSchedule --> UnitSymbol : BasicIntervalSchedule.value2Unit
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [BasicIntervalSchedule](BasicIntervalSchedule.md)
        * [RegularIntervalSchedule](RegularIntervalSchedule.md)
            * [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md)
                * **TapSchedule**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| TapChanger | [cim:TapSchedule.TapChanger](http://iec.ch/TC57/CIM100#TapSchedule.TapChanger) | 1 <br />  [TapChanger](TapChanger.md)  | A TapSchedule is associated with a TapChanger | direct |
| DayType | [cim:SeasonDayTypeSchedule.DayType](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule.DayType) | 1 <br />  [DayType](DayType.md)  | DayType for the Schedule | [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) |
| Season | [cim:SeasonDayTypeSchedule.Season](http://iec.ch/TC57/CIM100#SeasonDayTypeSchedule.Season) | 1 <br />  [Season](Season.md)  | Season for the Schedule | [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) |
| TimePoints | [cim:RegularIntervalSchedule.TimePoints](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.TimePoints) | 1..* <br />  [RegularTimePoint](RegularTimePoint.md)  | The regular interval time point data values that define this schedule | [RegularIntervalSchedule](RegularIntervalSchedule.md) |
| timeStep | [cim:RegularIntervalSchedule.timeStep](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.timeStep) | 1 <br />  [Seconds](Seconds.md)  | The time between each pair of subsequent regular time points in sequence orde... | [RegularIntervalSchedule](RegularIntervalSchedule.md) |
| endTime | [cim:RegularIntervalSchedule.endTime](http://iec.ch/TC57/CIM100#RegularIntervalSchedule.endTime) | 1 <br />  date  | The time for the last time point | [RegularIntervalSchedule](RegularIntervalSchedule.md) |
| startTime | [cim:BasicIntervalSchedule.startTime](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.startTime) | 1 <br />  date  | The time for the first time point | [BasicIntervalSchedule](BasicIntervalSchedule.md) |
| value1Unit | [cim:BasicIntervalSchedule.value1Unit](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.value1Unit) | 1 <br />  [UnitSymbol](UnitSymbol.md)  | Value1 units of measure | [BasicIntervalSchedule](BasicIntervalSchedule.md) |
| value2Unit | [cim:BasicIntervalSchedule.value2Unit](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.value2Unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | Value2 units of measure | [BasicIntervalSchedule](BasicIntervalSchedule.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [PhaseTapChanger](PhaseTapChanger.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [PhaseTapChangerAsymmetrical](PhaseTapChangerAsymmetrical.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [PhaseTapChangerLinear](PhaseTapChangerLinear.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [PhaseTapChangerSymmetrical](PhaseTapChangerSymmetrical.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [PhaseTapChangerTabular](PhaseTapChangerTabular.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [RatioTapChanger](RatioTapChanger.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |
| [TapChanger](TapChanger.md) | TapSchedules | range | [TapSchedule](TapSchedule.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:TapSchedule |
| native | this:TapSchedule |




