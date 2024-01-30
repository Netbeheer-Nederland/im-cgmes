# AccumulatorValue


_AccumulatorValue represents an accumulated (counted) MeasurementValue._





**URI**: [cim:AccumulatorValue](http://iec.ch/TC57/CIM100#AccumulatorValue)<br />
**Type**: Class




```mermaid
 classDiagram
    class AccumulatorValue
      MeasurementValue <|-- AccumulatorValue
      
      AccumulatorValue : AccumulatorValue.Accumulator
        
          AccumulatorValue --> Accumulator : AccumulatorValue.Accumulator
        
      AccumulatorValue : AccumulatorValue.AccumulatorReset
        
          AccumulatorValue --> AccumulatorReset : AccumulatorValue.AccumulatorReset
        
      AccumulatorValue : IdentifiedObject.description
        
      AccumulatorValue : MeasurementValue.MeasurementValueQuality
        
          AccumulatorValue --> MeasurementValueQuality : MeasurementValue.MeasurementValueQuality
        
      AccumulatorValue : MeasurementValue.MeasurementValueSource
        
          AccumulatorValue --> MeasurementValueSource : MeasurementValue.MeasurementValueSource
        
      AccumulatorValue : IdentifiedObject.mRID
        
      AccumulatorValue : IdentifiedObject.name
        
      AccumulatorValue : MeasurementValue.sensorAccuracy
        
          AccumulatorValue --> PerCent : MeasurementValue.sensorAccuracy
        
      AccumulatorValue : MeasurementValue.timeStamp
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [MeasurementValue](MeasurementValue.md)
            * **AccumulatorValue**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Accumulator | [cim:AccumulatorValue.Accumulator](http://iec.ch/TC57/CIM100#AccumulatorValue.Accumulator) | 1..1 <br />  [Accumulator](Accumulator.md)  | Measurement to which this value is connected | direct |
| AccumulatorReset | [cim:AccumulatorValue.AccumulatorReset](http://iec.ch/TC57/CIM100#AccumulatorValue.AccumulatorReset) | 0..1 <br />  [AccumulatorReset](AccumulatorReset.md)  | The command that resets the accumulator value | direct |
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
| [Accumulator](Accumulator.md) | AccumulatorValues | range | [AccumulatorValue](AccumulatorValue.md) |
| [AccumulatorReset](AccumulatorReset.md) | AccumulatorValue | range | [AccumulatorValue](AccumulatorValue.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AccumulatorValue |
| native | this:AccumulatorValue |




