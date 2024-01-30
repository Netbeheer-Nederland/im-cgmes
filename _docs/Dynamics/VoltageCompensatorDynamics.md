# VoltageCompensatorDynamics


_Voltage compensator function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:VoltageCompensatorDynamics](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class VoltageCompensatorDynamics
      DynamicsFunctionBlock <|-- VoltageCompensatorDynamics
      

      VoltageCompensatorDynamics <|-- VoltageCompensatorUserDefined
      VoltageCompensatorDynamics <|-- VCompIEEEType1
      VoltageCompensatorDynamics <|-- VCompIEEEType2
      
      
      VoltageCompensatorDynamics : IdentifiedObject.description
        
      VoltageCompensatorDynamics : DynamicsFunctionBlock.enabled
        
      VoltageCompensatorDynamics : VoltageCompensatorDynamics.ExcitationSystemDynamics
        
          VoltageCompensatorDynamics --> ExcitationSystemDynamics : VoltageCompensatorDynamics.ExcitationSystemDynamics
        
      VoltageCompensatorDynamics : IdentifiedObject.mRID
        
      VoltageCompensatorDynamics : IdentifiedObject.name
        
      VoltageCompensatorDynamics : VoltageCompensatorDynamics.RemoteInputSignal
        
          VoltageCompensatorDynamics --> RemoteInputSignal : VoltageCompensatorDynamics.RemoteInputSignal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **VoltageCompensatorDynamics**
            * [VoltageCompensatorUserDefined](VoltageCompensatorUserDefined.md)
            * [VCompIEEEType1](VCompIEEEType1.md)
            * [VCompIEEEType2](VCompIEEEType2.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RemoteInputSignal | [cim:VoltageCompensatorDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this voltage compensator model | direct |
| ExcitationSystemDynamics | [cim:VoltageCompensatorDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this voltage compensator is associated | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RemoteInputSignal](RemoteInputSignal.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcitationSystemUserDefined](ExcitationSystemUserDefined.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcitationSystemDynamics](ExcitationSystemDynamics.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC1A](ExcIEEEAC1A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC2A](ExcIEEEAC2A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC3A](ExcIEEEAC3A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC4A](ExcIEEEAC4A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC5A](ExcIEEEAC5A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC6A](ExcIEEEAC6A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC7B](ExcIEEEAC7B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEAC8B](ExcIEEEAC8B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEDC1A](ExcIEEEDC1A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEDC2A](ExcIEEEDC2A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEDC3A](ExcIEEEDC3A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEDC4B](ExcIEEEDC4B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST1A](ExcIEEEST1A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST2A](ExcIEEEST2A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST3A](ExcIEEEST3A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST4B](ExcIEEEST4B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST5B](ExcIEEEST5B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST6B](ExcIEEEST6B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcIEEEST7B](ExcIEEEST7B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC1A](ExcAC1A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC2A](ExcAC2A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC3A](ExcAC3A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC4A](ExcAC4A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC5A](ExcAC5A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC6A](ExcAC6A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAC8B](ExcAC8B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcANS](ExcANS.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAVR1](ExcAVR1.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAVR2](ExcAVR2.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAVR3](ExcAVR3.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAVR4](ExcAVR4.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAVR5](ExcAVR5.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcAVR7](ExcAVR7.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcBBC](ExcBBC.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcCZ](ExcCZ.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcDC1A](ExcDC1A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcDC2A](ExcDC2A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcDC3A](ExcDC3A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcDC3A1](ExcDC3A1.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcELIN1](ExcELIN1.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcELIN2](ExcELIN2.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcHU](ExcHU.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcNI](ExcNI.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcOEX3T](ExcOEX3T.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcPIC](ExcPIC.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcREXS](ExcREXS.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcRQB](ExcRQB.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcSCRX](ExcSCRX.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcSEXS](ExcSEXS.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcSK](ExcSK.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcST1A](ExcST1A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcST2A](ExcST2A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcST3A](ExcST3A.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcST4B](ExcST4B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcST6B](ExcST6B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| [ExcST7B](ExcST7B.md) | VoltageCompensatorDynamics | range | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VoltageCompensatorDynamics |
| native | this:VoltageCompensatorDynamics |




