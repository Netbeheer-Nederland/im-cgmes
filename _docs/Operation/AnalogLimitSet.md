# AnalogLimitSet


_An AnalogLimitSet specifies a set of Limits that are associated with an Analog measurement._





**URI**: [cim:AnalogLimitSet](http://iec.ch/TC57/CIM100#AnalogLimitSet)<br />
**Type**: Class




```mermaid
 classDiagram
    class AnalogLimitSet
      LimitSet <|-- AnalogLimitSet
      
      AnalogLimitSet : IdentifiedObject.description
        
      AnalogLimitSet : LimitSet.isPercentageLimits
        
      AnalogLimitSet : AnalogLimitSet.Limits
        
          AnalogLimitSet --> AnalogLimit : AnalogLimitSet.Limits
        
      AnalogLimitSet : AnalogLimitSet.Measurements
        
          AnalogLimitSet --> Analog : AnalogLimitSet.Measurements
        
      AnalogLimitSet : IdentifiedObject.mRID
        
      AnalogLimitSet : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [LimitSet](LimitSet.md)
        * **AnalogLimitSet**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Measurements | [cim:AnalogLimitSet.Measurements](http://iec.ch/TC57/CIM100#AnalogLimitSet.Measurements) | 1..* <br />  [Analog](Analog.md)  | The Measurements using the LimitSet | direct |
| Limits | [cim:AnalogLimitSet.Limits](http://iec.ch/TC57/CIM100#AnalogLimitSet.Limits) | 0..* <br />  [AnalogLimit](AnalogLimit.md)  | The limit values used for supervision of Measurements | direct |
| isPercentageLimits | [cim:LimitSet.isPercentageLimits](http://iec.ch/TC57/CIM100#LimitSet.isPercentageLimits) | 0..1 <br />  boolean  | Tells if the limit values are in percentage of normalValue or the specified U... | [LimitSet](LimitSet.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Analog](Analog.md) | LimitSets | range | [AnalogLimitSet](AnalogLimitSet.md) |
| [AnalogLimit](AnalogLimit.md) | LimitSet | range | [AnalogLimitSet](AnalogLimitSet.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AnalogLimitSet |
| native | this:AnalogLimitSet |




