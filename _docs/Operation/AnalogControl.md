# AnalogControl


_An analog control used for supervisory control._





**URI**: [cim:AnalogControl](http://iec.ch/TC57/CIM100#AnalogControl)<br />
**Type**: Class




```mermaid
 classDiagram
    class AnalogControl
    click AnalogControl href "../AnalogControl"
      Control <|-- AnalogControl
        click Control href "../Control"
      

      AnalogControl <|-- RaiseLowerCommand
        click RaiseLowerCommand href "../RaiseLowerCommand"
      AnalogControl <|-- SetPoint
        click SetPoint href "../SetPoint"
      
      
      AnalogControl : AnalogControl.AnalogValue
        
          AnalogControl --> AnalogValue : AnalogControl.AnalogValue
          click AnalogValue href "../AnalogValue"
        
      AnalogControl : Control.controlType
        
      AnalogControl : IdentifiedObject.description
        
      AnalogControl : AnalogControl.maxValue
        
      AnalogControl : AnalogControl.minValue
        
      AnalogControl : IdentifiedObject.mRID
        
      AnalogControl : IdentifiedObject.name
        
      AnalogControl : Control.operationInProgress
        
      AnalogControl : Control.PowerSystemResource
        
          AnalogControl --> PowerSystemResource : Control.PowerSystemResource
          click PowerSystemResource href "../PowerSystemResource"
        
      AnalogControl : Control.timeStamp
        
      AnalogControl : Control.unitMultiplier
        
          AnalogControl --> UnitMultiplier : Control.unitMultiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      AnalogControl : Control.unitSymbol
        
          AnalogControl --> UnitSymbol : Control.unitSymbol
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [Control](Control.md)
            * **AnalogControl**
                * [RaiseLowerCommand](RaiseLowerCommand.md)
                * [SetPoint](SetPoint.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| maxValue | [cim:AnalogControl.maxValue](http://iec.ch/TC57/CIM100#AnalogControl.maxValue) | 1 <br />  float  | Normal value range maximum for any of the Control | direct |
| minValue | [cim:AnalogControl.minValue](http://iec.ch/TC57/CIM100#AnalogControl.minValue) | 1 <br />  float  | Normal value range minimum for any of the Control | direct |
| AnalogValue | [cim:AnalogControl.AnalogValue](http://iec.ch/TC57/CIM100#AnalogControl.AnalogValue) | 1 <br />  [AnalogValue](AnalogValue.md)  | The MeasurementValue that is controlled | direct |
| controlType | [cim:Control.controlType](http://iec.ch/TC57/CIM100#Control.controlType) | 1 <br />  string  | Specifies the type of Control | [Control](Control.md) |
| operationInProgress | [cim:Control.operationInProgress](http://iec.ch/TC57/CIM100#Control.operationInProgress) | 0..1 <br />  boolean  | Indicates that a client is currently sending control commands that has not co... | [Control](Control.md) |
| timeStamp | [cim:Control.timeStamp](http://iec.ch/TC57/CIM100#Control.timeStamp) | 0..1 <br />  date  | The last time a control output was sent | [Control](Control.md) |
| unitMultiplier | [cim:Control.unitMultiplier](http://iec.ch/TC57/CIM100#Control.unitMultiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  | The unit multiplier of the controlled quantity | [Control](Control.md) |
| unitSymbol | [cim:Control.unitSymbol](http://iec.ch/TC57/CIM100#Control.unitSymbol) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | The unit of measure of the controlled quantity | [Control](Control.md) |
| PowerSystemResource | [cim:Control.PowerSystemResource](http://iec.ch/TC57/CIM100#Control.PowerSystemResource) | 0..1 <br />  [PowerSystemResource](PowerSystemResource.md)  | Regulating device governed by this control output | [Control](Control.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [AnalogValue](AnalogValue.md) | AnalogControl | range | [AnalogControl](AnalogControl.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AnalogControl |
| native | this:AnalogControl |




