# DiscontinuousExcitationControlDynamics


_Discontinuous excitation control function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model</font>._





**URI**: [cim:DiscontinuousExcitationControlDynamics](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class DiscontinuousExcitationControlDynamics
      DynamicsFunctionBlock <|-- DiscontinuousExcitationControlDynamics
      

      DiscontinuousExcitationControlDynamics <|-- DiscontinuousExcitationControlUserDefined
      DiscontinuousExcitationControlDynamics <|-- DiscExcContIEEEDEC1A
      DiscontinuousExcitationControlDynamics <|-- DiscExcContIEEEDEC2A
      DiscontinuousExcitationControlDynamics <|-- DiscExcContIEEEDEC3A
      
      
      DiscontinuousExcitationControlDynamics : IdentifiedObject.description
        
      DiscontinuousExcitationControlDynamics : DynamicsFunctionBlock.enabled
        
      DiscontinuousExcitationControlDynamics : DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics
        
          DiscontinuousExcitationControlDynamics --> ExcitationSystemDynamics : DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics
        
      DiscontinuousExcitationControlDynamics : IdentifiedObject.mRID
        
      DiscontinuousExcitationControlDynamics : IdentifiedObject.name
        
      DiscontinuousExcitationControlDynamics : DiscontinuousExcitationControlDynamics.RemoteInputSignal
        
          DiscontinuousExcitationControlDynamics --> RemoteInputSignal : DiscontinuousExcitationControlDynamics.RemoteInputSignal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **DiscontinuousExcitationControlDynamics**
            * [DiscontinuousExcitationControlUserDefined](DiscontinuousExcitationControlUserDefined.md)
            * [DiscExcContIEEEDEC1A](DiscExcContIEEEDEC1A.md)
            * [DiscExcContIEEEDEC2A](DiscExcContIEEEDEC2A.md)
            * [DiscExcContIEEEDEC3A](DiscExcContIEEEDEC3A.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RemoteInputSignal | [cim:DiscontinuousExcitationControlDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this discontinuous excitation control system mode... | direct |
| ExcitationSystemDynamics | [cim:DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this discontinuous excitation control mode... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RemoteInputSignal](RemoteInputSignal.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcitationSystemUserDefined](ExcitationSystemUserDefined.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcitationSystemDynamics](ExcitationSystemDynamics.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC1A](ExcIEEEAC1A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC2A](ExcIEEEAC2A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC3A](ExcIEEEAC3A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC4A](ExcIEEEAC4A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC5A](ExcIEEEAC5A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC6A](ExcIEEEAC6A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC7B](ExcIEEEAC7B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEAC8B](ExcIEEEAC8B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEDC1A](ExcIEEEDC1A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEDC2A](ExcIEEEDC2A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEDC3A](ExcIEEEDC3A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEDC4B](ExcIEEEDC4B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST1A](ExcIEEEST1A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST2A](ExcIEEEST2A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST3A](ExcIEEEST3A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST4B](ExcIEEEST4B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST5B](ExcIEEEST5B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST6B](ExcIEEEST6B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcIEEEST7B](ExcIEEEST7B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC1A](ExcAC1A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC2A](ExcAC2A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC3A](ExcAC3A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC4A](ExcAC4A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC5A](ExcAC5A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC6A](ExcAC6A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAC8B](ExcAC8B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcANS](ExcANS.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAVR1](ExcAVR1.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAVR2](ExcAVR2.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAVR3](ExcAVR3.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAVR4](ExcAVR4.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAVR5](ExcAVR5.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcAVR7](ExcAVR7.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcBBC](ExcBBC.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcCZ](ExcCZ.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcDC1A](ExcDC1A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcDC2A](ExcDC2A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcDC3A](ExcDC3A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcDC3A1](ExcDC3A1.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcELIN1](ExcELIN1.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcELIN2](ExcELIN2.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcHU](ExcHU.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcNI](ExcNI.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcOEX3T](ExcOEX3T.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcPIC](ExcPIC.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcREXS](ExcREXS.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcRQB](ExcRQB.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcSCRX](ExcSCRX.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcSEXS](ExcSEXS.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcSK](ExcSK.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcST1A](ExcST1A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcST2A](ExcST2A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcST3A](ExcST3A.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcST4B](ExcST4B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcST6B](ExcST6B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| [ExcST7B](ExcST7B.md) | DiscontinuousExcitationControlDynamics | range | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DiscontinuousExcitationControlDynamics |
| native | this:DiscontinuousExcitationControlDynamics |




