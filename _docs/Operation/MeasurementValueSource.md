# MeasurementValueSource


_MeasurementValueSource describes the alternative sources updating a MeasurementValue. User conventions for how to use the MeasurementValueSource attributes are defined in IEC 61970-301._





**URI**: [cim:MeasurementValueSource](http://iec.ch/TC57/CIM100#MeasurementValueSource)<br />
**Type**: Class




```mermaid
 classDiagram
    class MeasurementValueSource
    click MeasurementValueSource href "../MeasurementValueSource"
      IdentifiedObject <|-- MeasurementValueSource
        click IdentifiedObject href "../IdentifiedObject"
      
      MeasurementValueSource : IdentifiedObject.description
        
      MeasurementValueSource : MeasurementValueSource.MeasurementValues
        
          MeasurementValueSource --> MeasurementValue : MeasurementValueSource.MeasurementValues
          click MeasurementValue href "../MeasurementValue"
        
      MeasurementValueSource : IdentifiedObject.mRID
        
      MeasurementValueSource : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **MeasurementValueSource**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| MeasurementValues | [cim:MeasurementValueSource.MeasurementValues](http://iec.ch/TC57/CIM100#MeasurementValueSource.MeasurementValues) | * <br />  [MeasurementValue](MeasurementValue.md)  | The MeasurementValues updated by the source | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [AccumulatorValue](AccumulatorValue.md) | MeasurementValueSource | range | [MeasurementValueSource](MeasurementValueSource.md) |
| [AnalogValue](AnalogValue.md) | MeasurementValueSource | range | [MeasurementValueSource](MeasurementValueSource.md) |
| [DiscreteValue](DiscreteValue.md) | MeasurementValueSource | range | [MeasurementValueSource](MeasurementValueSource.md) |
| [MeasurementValue](MeasurementValue.md) | MeasurementValueSource | range | [MeasurementValueSource](MeasurementValueSource.md) |
| [StringMeasurementValue](StringMeasurementValue.md) | MeasurementValueSource | range | [MeasurementValueSource](MeasurementValueSource.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:MeasurementValueSource |
| native | this:MeasurementValueSource |




