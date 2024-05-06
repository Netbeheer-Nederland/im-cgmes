# IOPoint


_The class describe a measurement or control value. The purpose is to enable having attributes and associations common for measurement and control._





**URI**: [cim:IOPoint](http://iec.ch/TC57/CIM100#IOPoint)<br />
**Type**: Class




```mermaid
 classDiagram
    class IOPoint
    click IOPoint href "../IOPoint"
      IdentifiedObject <|-- IOPoint
        click IdentifiedObject href "../IdentifiedObject"
      

      IOPoint <|-- Control
        click Control href "../Control"
      IOPoint <|-- MeasurementValue
        click MeasurementValue href "../MeasurementValue"
      
      
      IOPoint : IdentifiedObject.description
        
      IOPoint : IdentifiedObject.mRID
        
      IOPoint : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **IOPoint**
        * [Control](Control.md)
        * [MeasurementValue](MeasurementValue.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:IOPoint |
| native | this:IOPoint |




