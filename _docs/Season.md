# Season


_A specified time period of the year._





**URI**: [cim:Season](http://iec.ch/TC57/CIM100#Season)<br />
**Type**: Class




```mermaid
 classDiagram
    class Season
      IdentifiedObject <|-- Season
      
      Season : IdentifiedObject.description
        
      Season : Season.endDate
        
      Season : IdentifiedObject.energyIdentCodeEic
        
      Season : IdentifiedObject.mRID
        
      Season : IdentifiedObject.name
        
      Season : Season.SeasonDayTypeSchedules
        
          Season --> SeasonDayTypeSchedule : Season.SeasonDayTypeSchedules
        
      Season : IdentifiedObject.shortName
        
      Season : Season.startDate
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **Season**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| endDate | [cim:Season.endDate](http://iec.ch/TC57/CIM100#Season.endDate) | 1..1 <br />  date  | Date season ends | direct |
| startDate | [cim:Season.startDate](http://iec.ch/TC57/CIM100#Season.startDate) | 1..1 <br />  date  | Date season starts | direct |
| SeasonDayTypeSchedules | [cim:Season.SeasonDayTypeSchedules](http://iec.ch/TC57/CIM100#Season.SeasonDayTypeSchedules) | 0..* <br />  [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md)  | Schedules that use this Season | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConformLoadSchedule](ConformLoadSchedule.md) | Season | range | [Season](Season.md) |
| [RegulationSchedule](RegulationSchedule.md) | Season | range | [Season](Season.md) |
| [TapSchedule](TapSchedule.md) | Season | range | [Season](Season.md) |
| [NonConformLoadSchedule](NonConformLoadSchedule.md) | Season | range | [Season](Season.md) |
| [SeasonDayTypeSchedule](SeasonDayTypeSchedule.md) | Season | range | [Season](Season.md) |
| [SwitchSchedule](SwitchSchedule.md) | Season | range | [Season](Season.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Season |
| native | this:Season |




