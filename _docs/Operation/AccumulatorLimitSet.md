# AccumulatorLimitSet


_An AccumulatorLimitSet specifies a set of Limits that are associated with an Accumulator measurement._





**URI**: [cim:AccumulatorLimitSet](http://iec.ch/TC57/CIM100#AccumulatorLimitSet)<br />
**Type**: Class




```mermaid
 classDiagram
    class AccumulatorLimitSet
    click AccumulatorLimitSet href "../AccumulatorLimitSet"
      LimitSet <|-- AccumulatorLimitSet
        click LimitSet href "../LimitSet"
      
      AccumulatorLimitSet : IdentifiedObject.description
        
      AccumulatorLimitSet : LimitSet.isPercentageLimits
        
      AccumulatorLimitSet : AccumulatorLimitSet.Limits
        
          AccumulatorLimitSet --> AccumulatorLimit : AccumulatorLimitSet.Limits
          click AccumulatorLimit href "../AccumulatorLimit"
        
      AccumulatorLimitSet : AccumulatorLimitSet.Measurements
        
          AccumulatorLimitSet --> Accumulator : AccumulatorLimitSet.Measurements
          click Accumulator href "../Accumulator"
        
      AccumulatorLimitSet : IdentifiedObject.mRID
        
      AccumulatorLimitSet : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [LimitSet](LimitSet.md)
        * **AccumulatorLimitSet**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Measurements | [cim:AccumulatorLimitSet.Measurements](http://iec.ch/TC57/CIM100#AccumulatorLimitSet.Measurements) | 1..* <br />  [Accumulator](Accumulator.md)  | The Measurements using the LimitSet | direct |
| Limits | [cim:AccumulatorLimitSet.Limits](http://iec.ch/TC57/CIM100#AccumulatorLimitSet.Limits) | 1..* <br />  [AccumulatorLimit](AccumulatorLimit.md)  | The limit values used for supervision of Measurements | direct |
| isPercentageLimits | [cim:LimitSet.isPercentageLimits](http://iec.ch/TC57/CIM100#LimitSet.isPercentageLimits) | 0..1 <br />  boolean  | Tells if the limit values are in percentage of normalValue or the specified U... | [LimitSet](LimitSet.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Accumulator](Accumulator.md) | LimitSets | range | [AccumulatorLimitSet](AccumulatorLimitSet.md) |
| [AccumulatorLimit](AccumulatorLimit.md) | LimitSet | range | [AccumulatorLimitSet](AccumulatorLimitSet.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AccumulatorLimitSet |
| native | this:AccumulatorLimitSet |




