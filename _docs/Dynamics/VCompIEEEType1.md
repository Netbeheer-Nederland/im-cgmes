# VCompIEEEType1


_<font color="#0f0f0f">Terminal voltage transducer and load compensator as defined in IEEE 421.5-2005, 4. This model is common to all excitation system models described in the IEEE Standard. </font>_

_<font color="#0f0f0f">Parameter details:</font>_

_<ol>_

_	<li><font color="#0f0f0f">If <i>Rc</i> and <i>Xc</i> are set to zero, the l</font>oad compensation is not employed and the behaviour is as a simple sensing circuit.</li>_

_</ol>_

_<ol>_

_	<li>If all parameters (<i>Rc</i>, <i>Xc</i> and <i>Tr</i>) are set to zero, the standard model VCompIEEEType1 is bypassed.</li>_

_</ol>_

_Reference: IEEE 421.5-2005 4._





**URI**: [cim:VCompIEEEType1](http://iec.ch/TC57/CIM100#VCompIEEEType1)<br />
**Type**: Class




```mermaid
 classDiagram
    class VCompIEEEType1
    click VCompIEEEType1 href "../VCompIEEEType1"
      VoltageCompensatorDynamics <|-- VCompIEEEType1
        click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
      
      VCompIEEEType1 : IdentifiedObject.description
        
      VCompIEEEType1 : DynamicsFunctionBlock.enabled
        
      VCompIEEEType1 : VoltageCompensatorDynamics.ExcitationSystemDynamics
        
          VCompIEEEType1 --> ExcitationSystemDynamics : VoltageCompensatorDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      VCompIEEEType1 : IdentifiedObject.mRID
        
      VCompIEEEType1 : IdentifiedObject.name
        
      VCompIEEEType1 : VCompIEEEType1.rc
        
          VCompIEEEType1 --> PU : VCompIEEEType1.rc
          click PU href "../PU"
        
      VCompIEEEType1 : VoltageCompensatorDynamics.RemoteInputSignal
        
          VCompIEEEType1 --> RemoteInputSignal : VoltageCompensatorDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      VCompIEEEType1 : VCompIEEEType1.tr
        
          VCompIEEEType1 --> Seconds : VCompIEEEType1.tr
          click Seconds href "../Seconds"
        
      VCompIEEEType1 : VCompIEEEType1.xc
        
          VCompIEEEType1 --> PU : VCompIEEEType1.xc
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)
            * **VCompIEEEType1**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| rc | [cim:VCompIEEEType1.rc](http://iec.ch/TC57/CIM100#VCompIEEEType1.rc) | 1 <br />  [PU](PU.md)  | <font color="#0f0f0f">Resistive component of compensation of a generator (<i>... | direct |
| xc | [cim:VCompIEEEType1.xc](http://iec.ch/TC57/CIM100#VCompIEEEType1.xc) | 1 <br />  [PU](PU.md)  | <font color="#0f0f0f">Reactive component of compensation of a generator (<i>X... | direct |
| tr | [cim:VCompIEEEType1.tr](http://iec.ch/TC57/CIM100#VCompIEEEType1.tr) | 1 <br />  [Seconds](Seconds.md)  | <font color="#0f0f0f">Time constant which is used for the combined voltage se... | direct |
| RemoteInputSignal | [cim:VoltageCompensatorDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this voltage compensator model | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| ExcitationSystemDynamics | [cim:VoltageCompensatorDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this voltage compensator is associated | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VCompIEEEType1 |
| native | this:VCompIEEEType1 |




