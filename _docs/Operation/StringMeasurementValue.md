# StringMeasurementValue


_StringMeasurementValue represents a measurement value of type string._





**URI**: [cim:StringMeasurementValue](http://iec.ch/TC57/CIM100#StringMeasurementValue)<br />
**Type**: Class




```mermaid
 classDiagram
    class StringMeasurementValue
    click StringMeasurementValue href "../StringMeasurementValue"
      MeasurementValue <|-- StringMeasurementValue
        click MeasurementValue href "../MeasurementValue"
      
      StringMeasurementValue : IdentifiedObject.description
        
      StringMeasurementValue : MeasurementValue.MeasurementValueQuality
        
          StringMeasurementValue --> MeasurementValueQuality : MeasurementValue.MeasurementValueQuality
          click MeasurementValueQuality href "../MeasurementValueQuality"
        
      StringMeasurementValue : MeasurementValue.MeasurementValueSource
        
          StringMeasurementValue --> MeasurementValueSource : MeasurementValue.MeasurementValueSource
          click MeasurementValueSource href "../MeasurementValueSource"
        
      StringMeasurementValue : IdentifiedObject.mRID
        
      StringMeasurementValue : IdentifiedObject.name
        
      StringMeasurementValue : MeasurementValue.sensorAccuracy
        
          StringMeasurementValue --> PerCent : MeasurementValue.sensorAccuracy
          click PerCent href "../PerCent"
        
      StringMeasurementValue : StringMeasurementValue.StringMeasurement
        
          StringMeasurementValue --> StringMeasurement : StringMeasurementValue.StringMeasurement
          click StringMeasurement href "../StringMeasurement"
        
      StringMeasurementValue : MeasurementValue.timeStamp
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [MeasurementValue](MeasurementValue.md)
            * **StringMeasurementValue**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| StringMeasurement | [cim:StringMeasurementValue.StringMeasurement](http://iec.ch/TC57/CIM100#StringMeasurementValue.StringMeasurement) | 1 <br />  [StringMeasurement](StringMeasurement.md)  | Measurement to which this value is connected | direct |
| timeStamp | [cim:MeasurementValue.timeStamp](http://iec.ch/TC57/CIM100#MeasurementValue.timeStamp) | 0..1 <br />  date  | The time when the value was last updated | [MeasurementValue](MeasurementValue.md) |
| sensorAccuracy | [cim:MeasurementValue.sensorAccuracy](http://iec.ch/TC57/CIM100#MeasurementValue.sensorAccuracy) | 0..1 <br />  [PerCent](PerCent.md)  | The limit, expressed as a percentage of the sensor maximum, that errors will ... | [MeasurementValue](MeasurementValue.md) |
| MeasurementValueQuality | [cim:MeasurementValue.MeasurementValueQuality](http://iec.ch/TC57/CIM100#MeasurementValue.MeasurementValueQuality) | 0..1 <br />  [MeasurementValueQuality](MeasurementValueQuality.md)  | A MeasurementValue has a MeasurementValueQuality associated with it | [MeasurementValue](MeasurementValue.md) |
| MeasurementValueSource | [cim:MeasurementValue.MeasurementValueSource](http://iec.ch/TC57/CIM100#MeasurementValue.MeasurementValueSource) | 1 <br />  [MeasurementValueSource](MeasurementValueSource.md)  | A reference to the type of source that updates the MeasurementValue, e | [MeasurementValue](MeasurementValue.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [StringMeasurement](StringMeasurement.md) | StringMeasurementValues | range | [StringMeasurementValue](StringMeasurementValue.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:StringMeasurementValue |
| native | this:StringMeasurementValue |




