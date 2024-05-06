# IdentifiedObject


_This is a root class to provide common identification for all classes needing identification and naming attributes._





**URI**: [cim:IdentifiedObject](http://iec.ch/TC57/CIM100#IdentifiedObject)<br />
**Type**: Class




```mermaid
 classDiagram
    class IdentifiedObject
    click IdentifiedObject href "../IdentifiedObject"
      IdentifiedObject <|-- ACDCTerminal
        click ACDCTerminal href "../ACDCTerminal"
      IdentifiedObject <|-- IOPoint
        click IOPoint href "../IOPoint"
      IdentifiedObject <|-- Limit
        click Limit href "../Limit"
      IdentifiedObject <|-- LimitSet
        click LimitSet href "../LimitSet"
      IdentifiedObject <|-- Measurement
        click Measurement href "../Measurement"
      IdentifiedObject <|-- MeasurementValueSource
        click MeasurementValueSource href "../MeasurementValueSource"
      IdentifiedObject <|-- PowerSystemResource
        click PowerSystemResource href "../PowerSystemResource"
      IdentifiedObject <|-- ValueAliasSet
        click ValueAliasSet href "../ValueAliasSet"
      IdentifiedObject <|-- ValueToAlias
        click ValueToAlias href "../ValueToAlias"
      
      IdentifiedObject : IdentifiedObject.description
        
      IdentifiedObject : IdentifiedObject.mRID
        
      IdentifiedObject : IdentifiedObject.name
        
      
```





## Inheritance
* **IdentifiedObject**
    * [ACDCTerminal](ACDCTerminal.md)
    * [IOPoint](IOPoint.md)
    * [Limit](Limit.md)
    * [LimitSet](LimitSet.md)
    * [Measurement](Measurement.md)
    * [MeasurementValueSource](MeasurementValueSource.md)
    * [PowerSystemResource](PowerSystemResource.md)
    * [ValueAliasSet](ValueAliasSet.md)
    * [ValueToAlias](ValueToAlias.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | direct |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | direct |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:IdentifiedObject |
| native | this:IdentifiedObject |




