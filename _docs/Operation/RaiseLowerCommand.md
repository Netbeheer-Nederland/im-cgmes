# RaiseLowerCommand


_An analog control that increases or decreases a set point value with pulses. Unless otherwise specified, one pulse moves the set point by one._





**URI**: [cim:RaiseLowerCommand](http://iec.ch/TC57/CIM100#RaiseLowerCommand)<br />
**Type**: Class




```mermaid
 classDiagram
    class RaiseLowerCommand
      AnalogControl <|-- RaiseLowerCommand
      
      RaiseLowerCommand : AnalogControl.AnalogValue
        
          RaiseLowerCommand --> AnalogValue : AnalogControl.AnalogValue
        
      RaiseLowerCommand : Control.controlType
        
      RaiseLowerCommand : IdentifiedObject.description
        
      RaiseLowerCommand : AnalogControl.maxValue
        
      RaiseLowerCommand : AnalogControl.minValue
        
      RaiseLowerCommand : IdentifiedObject.mRID
        
      RaiseLowerCommand : IdentifiedObject.name
        
      RaiseLowerCommand : Control.operationInProgress
        
      RaiseLowerCommand : Control.PowerSystemResource
        
          RaiseLowerCommand --> PowerSystemResource : Control.PowerSystemResource
        
      RaiseLowerCommand : Control.timeStamp
        
      RaiseLowerCommand : Control.unitMultiplier
        
          RaiseLowerCommand --> UnitMultiplier : Control.unitMultiplier
        
      RaiseLowerCommand : Control.unitSymbol
        
          RaiseLowerCommand --> UnitSymbol : Control.unitSymbol
        
      RaiseLowerCommand : RaiseLowerCommand.ValueAliasSet
        
          RaiseLowerCommand --> ValueAliasSet : RaiseLowerCommand.ValueAliasSet
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [Control](Control.md)
            * [AnalogControl](AnalogControl.md)
                * **RaiseLowerCommand**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ValueAliasSet | [cim:RaiseLowerCommand.ValueAliasSet](http://iec.ch/TC57/CIM100#RaiseLowerCommand.ValueAliasSet) | 0..1 <br />  [ValueAliasSet](ValueAliasSet.md)  | The ValueAliasSet used for translation of a Control value to a name | direct |
| maxValue | [cim:AnalogControl.maxValue](http://iec.ch/TC57/CIM100#AnalogControl.maxValue) | 1..1 <br />  float  | Normal value range maximum for any of the Control | [AnalogControl](AnalogControl.md) |
| minValue | [cim:AnalogControl.minValue](http://iec.ch/TC57/CIM100#AnalogControl.minValue) | 1..1 <br />  float  | Normal value range minimum for any of the Control | [AnalogControl](AnalogControl.md) |
| AnalogValue | [cim:AnalogControl.AnalogValue](http://iec.ch/TC57/CIM100#AnalogControl.AnalogValue) | 1..1 <br />  [AnalogValue](AnalogValue.md)  | The MeasurementValue that is controlled | [AnalogControl](AnalogControl.md) |
| controlType | [cim:Control.controlType](http://iec.ch/TC57/CIM100#Control.controlType) | 1..1 <br />  string  | Specifies the type of Control | [Control](Control.md) |
| operationInProgress | [cim:Control.operationInProgress](http://iec.ch/TC57/CIM100#Control.operationInProgress) | 0..1 <br />  boolean  | Indicates that a client is currently sending control commands that has not co... | [Control](Control.md) |
| timeStamp | [cim:Control.timeStamp](http://iec.ch/TC57/CIM100#Control.timeStamp) | 0..1 <br />  date  | The last time a control output was sent | [Control](Control.md) |
| unitMultiplier | [cim:Control.unitMultiplier](http://iec.ch/TC57/CIM100#Control.unitMultiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  | The unit multiplier of the controlled quantity | [Control](Control.md) |
| unitSymbol | [cim:Control.unitSymbol](http://iec.ch/TC57/CIM100#Control.unitSymbol) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | The unit of measure of the controlled quantity | [Control](Control.md) |
| PowerSystemResource | [cim:Control.PowerSystemResource](http://iec.ch/TC57/CIM100#Control.PowerSystemResource) | 0..1 <br />  [PowerSystemResource](PowerSystemResource.md)  | Regulating device governed by this control output | [Control](Control.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ValueAliasSet](ValueAliasSet.md) | RaiseLowerCommands | range | [RaiseLowerCommand](RaiseLowerCommand.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RaiseLowerCommand |
| native | this:RaiseLowerCommand |




