# Command


_A Command is a discrete control used for supervisory control._





**URI**: [cim:Command](http://iec.ch/TC57/CIM100#Command)<br />
**Type**: Class




```mermaid
 classDiagram
    class Command
      Control <|-- Command
      
      Command : Control.controlType
        
      Command : IdentifiedObject.description
        
      Command : Command.DiscreteValue
        
          Command --> DiscreteValue : Command.DiscreteValue
        
      Command : IdentifiedObject.mRID
        
      Command : IdentifiedObject.name
        
      Command : Command.normalValue
        
      Command : Control.operationInProgress
        
      Command : Control.PowerSystemResource
        
          Command --> PowerSystemResource : Control.PowerSystemResource
        
      Command : Control.timeStamp
        
      Command : Control.unitMultiplier
        
          Command --> UnitMultiplier : Control.unitMultiplier
        
      Command : Control.unitSymbol
        
          Command --> UnitSymbol : Control.unitSymbol
        
      Command : Command.value
        
      Command : Command.ValueAliasSet
        
          Command --> ValueAliasSet : Command.ValueAliasSet
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [IOPoint](IOPoint.md)
        * [Control](Control.md)
            * **Command**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| normalValue | [cim:Command.normalValue](http://iec.ch/TC57/CIM100#Command.normalValue) | 1..1 <br />  integer  | Normal value for Control | direct |
| value | [cim:Command.value](http://iec.ch/TC57/CIM100#Command.value) | 1..1 <br />  integer  | The value representing the actuator output | direct |
| ValueAliasSet | [cim:Command.ValueAliasSet](http://iec.ch/TC57/CIM100#Command.ValueAliasSet) | 0..1 <br />  [ValueAliasSet](ValueAliasSet.md)  | The ValueAliasSet used for translation of a Control value to a name | direct |
| DiscreteValue | [cim:Command.DiscreteValue](http://iec.ch/TC57/CIM100#Command.DiscreteValue) | 1..1 <br />  [DiscreteValue](DiscreteValue.md)  | The MeasurementValue that is controlled | direct |
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
| [DiscreteValue](DiscreteValue.md) | Command | range | [Command](Command.md) |
| [ValueAliasSet](ValueAliasSet.md) | Commands | range | [Command](Command.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Command |
| native | this:Command |




