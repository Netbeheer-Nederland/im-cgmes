# DiscreteValue


_DiscreteValue represents a discrete MeasurementValue._





**URI**: [cim:DiscreteValue](http://iec.ch/TC57/CIM100#DiscreteValue)<br />
**Type**: Class




```mermaid
 classDiagram
    class DiscreteValue
    click DiscreteValue href "../DiscreteValue"
      MeasurementValue <|-- DiscreteValue
        click MeasurementValue href "../MeasurementValue"
      
      DiscreteValue : DiscreteValue.Command
        
          DiscreteValue --> Command : DiscreteValue.Command
          click Command href "../Command"
        
      DiscreteValue : IdentifiedObject.description
        
      DiscreteValue : DiscreteValue.Discrete
        
          DiscreteValue --> Discrete : DiscreteValue.Discrete
          click Discrete href "../Discrete"
        
      DiscreteValue : MeasurementValue.MeasurementValueQuality
        
          DiscreteValue --> MeasurementValueQuality : MeasurementValue.MeasurementValueQuality
          click MeasurementValueQuality href "../MeasurementValueQuality"
        
      DiscreteValue : MeasurementValue.MeasurementValueSource
        
          DiscreteValue --> MeasurementValueSource : MeasurementValue.MeasurementValueSource
          click MeasurementValueSource href "../MeasurementValueSource"
        
      DiscreteValue : IdentifiedObject.mRID
        
      DiscreteValue : IdentifiedObject.name
        
      DiscreteValue : MeasurementValue.sensorAccuracy
        
          DiscreteValue --> PerCent : MeasurementValue.sensorAccuracy
          click PerCent href "../PerCent"
        
      DiscreteValue : MeasurementValue.timeStamp
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [MeasurementValue](MeasurementValue.md)
            * **DiscreteValue**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Command | [cim:DiscreteValue.Command](http://iec.ch/TC57/CIM100#DiscreteValue.Command) | 0..1 <br />  [Command](Command.md)  | The Control variable associated with the MeasurementValue | direct |
| Discrete | [cim:DiscreteValue.Discrete](http://iec.ch/TC57/CIM100#DiscreteValue.Discrete) | 1 <br />  [Discrete](Discrete.md)  | Measurement to which this value is connected | direct |
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
| [Command](Command.md) | DiscreteValue | range | [DiscreteValue](DiscreteValue.md) |
| [Discrete](Discrete.md) | DiscreteValues | range | [DiscreteValue](DiscreteValue.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DiscreteValue |
| native | this:DiscreteValue |




