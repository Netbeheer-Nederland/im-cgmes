# VCompIEEEType2


_<font color="#0f0f0f">Terminal voltage transducer and load compensator as defined in IEEE 421.5-2005, 4. This model is designed to cover the following types of compensation: </font>_

_<ul>_

_	<li><font color="#0f0f0f">reactive droop;</font></li>_

_	<li><font color="#0f0f0f">transformer-drop or line-drop compensation;</font></li>_

_	<li><font color="#0f0f0f">reactive differential compensation known also as cross-current compensation.</font></li>_

_</ul>_

_<font color="#0f0f0f">Reference: IEEE 421.5-2005, 4.</font>_





**URI**: [cim:VCompIEEEType2](http://iec.ch/TC57/CIM100#VCompIEEEType2)<br />
**Type**: Class




```mermaid
 classDiagram
    class VCompIEEEType2
    click VCompIEEEType2 href "../VCompIEEEType2"
      VoltageCompensatorDynamics <|-- VCompIEEEType2
        click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
      
      VCompIEEEType2 : IdentifiedObject.description
        
      VCompIEEEType2 : DynamicsFunctionBlock.enabled
        
      VCompIEEEType2 : VoltageCompensatorDynamics.ExcitationSystemDynamics
        
          VCompIEEEType2 --> ExcitationSystemDynamics : VoltageCompensatorDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      VCompIEEEType2 : VCompIEEEType2.GenICompensationForGenJ
        
          VCompIEEEType2 --> GenICompensationForGenJ : VCompIEEEType2.GenICompensationForGenJ
          click GenICompensationForGenJ href "../GenICompensationForGenJ"
        
      VCompIEEEType2 : IdentifiedObject.mRID
        
      VCompIEEEType2 : IdentifiedObject.name
        
      VCompIEEEType2 : VoltageCompensatorDynamics.RemoteInputSignal
        
          VCompIEEEType2 --> RemoteInputSignal : VoltageCompensatorDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      VCompIEEEType2 : VCompIEEEType2.tr
        
          VCompIEEEType2 --> Seconds : VCompIEEEType2.tr
          click Seconds href "../Seconds"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)
            * **VCompIEEEType2**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| tr | [cim:VCompIEEEType2.tr](http://iec.ch/TC57/CIM100#VCompIEEEType2.tr) | 1 <br />  [Seconds](Seconds.md)  | <font color="#0f0f0f">Time constant which is used for the combined voltage se... | direct |
| GenICompensationForGenJ | [cim:VCompIEEEType2.GenICompensationForGenJ](http://iec.ch/TC57/CIM100#VCompIEEEType2.GenICompensationForGenJ) | 1..* <br />  [GenICompensationForGenJ](GenICompensationForGenJ.md)  | Compensation of this voltage compensator's generator for current flow out of ... | direct |
| RemoteInputSignal | [cim:VoltageCompensatorDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this voltage compensator model | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| ExcitationSystemDynamics | [cim:VoltageCompensatorDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this voltage compensator is associated | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [GenICompensationForGenJ](GenICompensationForGenJ.md) | VcompIEEEType2 | range | [VCompIEEEType2](VCompIEEEType2.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VCompIEEEType2 |
| native | this:VCompIEEEType2 |




