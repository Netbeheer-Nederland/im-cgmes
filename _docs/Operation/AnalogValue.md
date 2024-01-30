# AnalogValue


_AnalogValue represents an analog MeasurementValue._





**URI**: [cim:AnalogValue](http://iec.ch/TC57/CIM100#AnalogValue)<br />
**Type**: Class




```mermaid
 classDiagram
    class AnalogValue
      MeasurementValue <|-- AnalogValue
      
      AnalogValue : AnalogValue.Analog
        
          AnalogValue --> Analog : AnalogValue.Analog
        
      AnalogValue : AnalogValue.AnalogControl
        
          AnalogValue --> AnalogControl : AnalogValue.AnalogControl
        
      AnalogValue : IdentifiedObject.description
        
      AnalogValue : MeasurementValue.MeasurementValueQuality
        
          AnalogValue --> MeasurementValueQuality : MeasurementValue.MeasurementValueQuality
        
      AnalogValue : MeasurementValue.MeasurementValueSource
        
          AnalogValue --> MeasurementValueSource : MeasurementValue.MeasurementValueSource
        
      AnalogValue : IdentifiedObject.mRID
        
      AnalogValue : IdentifiedObject.name
        
      AnalogValue : MeasurementValue.sensorAccuracy
        
          AnalogValue --> PerCent : MeasurementValue.sensorAccuracy
        
      AnalogValue : MeasurementValue.timeStamp
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [MeasurementValue](MeasurementValue.md)
            * **AnalogValue**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Analog | [cim:AnalogValue.Analog](http://iec.ch/TC57/CIM100#AnalogValue.Analog) | 1..1 <br />  [Analog](Analog.md)  | Measurement to which this value is connected | direct |
| AnalogControl | [cim:AnalogValue.AnalogControl](http://iec.ch/TC57/CIM100#AnalogValue.AnalogControl) | 0..1 <br />  [AnalogControl](AnalogControl.md)  | The Control variable associated with the MeasurementValue | direct |
| timeStamp | [cim:MeasurementValue.timeStamp](http://iec.ch/TC57/CIM100#MeasurementValue.timeStamp) | 0..1 <br />  date  | The time when the value was last updated | [MeasurementValue](MeasurementValue.md) |
| sensorAccuracy | [cim:MeasurementValue.sensorAccuracy](http://iec.ch/TC57/CIM100#MeasurementValue.sensorAccuracy) | 0..1 <br />  [PerCent](PerCent.md)  | The limit, expressed as a percentage of the sensor maximum, that errors will ... | [MeasurementValue](MeasurementValue.md) |
| MeasurementValueQuality | [cim:MeasurementValue.MeasurementValueQuality](http://iec.ch/TC57/CIM100#MeasurementValue.MeasurementValueQuality) | 0..1 <br />  [MeasurementValueQuality](MeasurementValueQuality.md)  | A MeasurementValue has a MeasurementValueQuality associated with it | [MeasurementValue](MeasurementValue.md) |
| MeasurementValueSource | [cim:MeasurementValue.MeasurementValueSource](http://iec.ch/TC57/CIM100#MeasurementValue.MeasurementValueSource) | 1..1 <br />  [MeasurementValueSource](MeasurementValueSource.md)  | A reference to the type of source that updates the MeasurementValue, e | [MeasurementValue](MeasurementValue.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Analog](Analog.md) | AnalogValues | range | [AnalogValue](AnalogValue.md) |
| [AnalogControl](AnalogControl.md) | AnalogValue | range | [AnalogValue](AnalogValue.md) |
| [RaiseLowerCommand](RaiseLowerCommand.md) | AnalogValue | range | [AnalogValue](AnalogValue.md) |
| [SetPoint](SetPoint.md) | AnalogValue | range | [AnalogValue](AnalogValue.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AnalogValue |
| native | this:AnalogValue |




