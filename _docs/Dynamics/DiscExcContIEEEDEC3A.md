# DiscExcContIEEEDEC3A


_IEEE type DEC3A model. In some systems, the stabilizer output is disconnected from the regulator immediately following a severe fault to prevent the stabilizer from competing with action of voltage regulator during the first swing._

_Reference: IEEE 421.5-2005 12.4._





**URI**: [cim:DiscExcContIEEEDEC3A](http://iec.ch/TC57/CIM100#DiscExcContIEEEDEC3A)<br />
**Type**: Class




```mermaid
 classDiagram
    class DiscExcContIEEEDEC3A
    click DiscExcContIEEEDEC3A href "../DiscExcContIEEEDEC3A"
      DiscontinuousExcitationControlDynamics <|-- DiscExcContIEEEDEC3A
        click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
      
      DiscExcContIEEEDEC3A : IdentifiedObject.description
        
      DiscExcContIEEEDEC3A : DynamicsFunctionBlock.enabled
        
      DiscExcContIEEEDEC3A : DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics
        
          DiscExcContIEEEDEC3A --> ExcitationSystemDynamics : DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      DiscExcContIEEEDEC3A : IdentifiedObject.mRID
        
      DiscExcContIEEEDEC3A : IdentifiedObject.name
        
      DiscExcContIEEEDEC3A : DiscontinuousExcitationControlDynamics.RemoteInputSignal
        
          DiscExcContIEEEDEC3A --> RemoteInputSignal : DiscontinuousExcitationControlDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      DiscExcContIEEEDEC3A : DiscExcContIEEEDEC3A.tdr
        
          DiscExcContIEEEDEC3A --> Seconds : DiscExcContIEEEDEC3A.tdr
          click Seconds href "../Seconds"
        
      DiscExcContIEEEDEC3A : DiscExcContIEEEDEC3A.vtmin
        
          DiscExcContIEEEDEC3A --> PU : DiscExcContIEEEDEC3A.vtmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md)
            * **DiscExcContIEEEDEC3A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| vtmin | [cim:DiscExcContIEEEDEC3A.vtmin](http://iec.ch/TC57/CIM100#DiscExcContIEEEDEC3A.vtmin) | 1 <br />  [PU](PU.md)  | Terminal undervoltage comparison level (<i>V</i><i><sub>TMIN</sub></i>) | direct |
| tdr | [cim:DiscExcContIEEEDEC3A.tdr](http://iec.ch/TC57/CIM100#DiscExcContIEEEDEC3A.tdr) | 1 <br />  [Seconds](Seconds.md)  | Reset time delay (<i>T</i><i><sub>DR</sub></i>) (&gt;= 0) | direct |
| RemoteInputSignal | [cim:DiscontinuousExcitationControlDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this discontinuous excitation control system mode... | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| ExcitationSystemDynamics | [cim:DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this discontinuous excitation control mode... | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
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
| self | cim:DiscExcContIEEEDEC3A |
| native | this:DiscExcContIEEEDEC3A |




