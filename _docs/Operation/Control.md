# Control


_Control is used for supervisory/device control. It represents control outputs that are used to change the state in a process, e.g. close or open breaker, a set point value or a raise lower command._





**URI**: [cim:Control](http://iec.ch/TC57/CIM100#Control)<br />
**Type**: Class




```mermaid
 classDiagram
    class Control
      IOPoint <|-- Control
      

      Control <|-- AccumulatorReset
      Control <|-- AnalogControl
      Control <|-- Command
      
      
      Control : Control.controlType
        
      Control : IdentifiedObject.description
        
      Control : IdentifiedObject.mRID
        
      Control : IdentifiedObject.name
        
      Control : Control.operationInProgress
        
      Control : Control.PowerSystemResource
        
          Control --> PowerSystemResource : Control.PowerSystemResource
        
      Control : Control.timeStamp
        
      Control : Control.unitMultiplier
        
          Control --> UnitMultiplier : Control.unitMultiplier
        
      Control : Control.unitSymbol
        
          Control --> UnitSymbol : Control.unitSymbol
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * **Control**
            * [AccumulatorReset](AccumulatorReset.md)
            * [AnalogControl](AnalogControl.md)
            * [Command](Command.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| controlType | [cim:Control.controlType](http://iec.ch/TC57/CIM100#Control.controlType) | 1..1 <br />  string  | Specifies the type of Control | direct |
| operationInProgress | [cim:Control.operationInProgress](http://iec.ch/TC57/CIM100#Control.operationInProgress) | 0..1 <br />  boolean  | Indicates that a client is currently sending control commands that has not co... | direct |
| timeStamp | [cim:Control.timeStamp](http://iec.ch/TC57/CIM100#Control.timeStamp) | 0..1 <br />  date  | The last time a control output was sent | direct |
| unitMultiplier | [cim:Control.unitMultiplier](http://iec.ch/TC57/CIM100#Control.unitMultiplier) | 0..1 <br />  [UnitMultiplier](UnitMultiplier.md)  | The unit multiplier of the controlled quantity | direct |
| unitSymbol | [cim:Control.unitSymbol](http://iec.ch/TC57/CIM100#Control.unitSymbol) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | The unit of measure of the controlled quantity | direct |
| PowerSystemResource | [cim:Control.PowerSystemResource](http://iec.ch/TC57/CIM100#Control.PowerSystemResource) | 0..1 <br />  [PowerSystemResource](PowerSystemResource.md)  | Regulating device governed by this control output | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [PowerSystemResource](PowerSystemResource.md) | Controls | range | [Control](Control.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Control |
| native | this:Control |




