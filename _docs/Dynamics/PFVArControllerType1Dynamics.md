# PFVArControllerType1Dynamics


_Power factor or VAr controller type 1 function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class PFVArControllerType1Dynamics
      DynamicsFunctionBlock <|-- PFVArControllerType1Dynamics
      

      PFVArControllerType1Dynamics <|-- PFVArControllerType1UserDefined
      PFVArControllerType1Dynamics <|-- PFVArType1IEEEPFController
      PFVArControllerType1Dynamics <|-- PFVArType1IEEEVArController
      
      
      PFVArControllerType1Dynamics : IdentifiedObject.description
        
      PFVArControllerType1Dynamics : DynamicsFunctionBlock.enabled
        
      PFVArControllerType1Dynamics : PFVArControllerType1Dynamics.ExcitationSystemDynamics
        
          PFVArControllerType1Dynamics --> ExcitationSystemDynamics : PFVArControllerType1Dynamics.ExcitationSystemDynamics
        
      PFVArControllerType1Dynamics : IdentifiedObject.mRID
        
      PFVArControllerType1Dynamics : IdentifiedObject.name
        
      PFVArControllerType1Dynamics : PFVArControllerType1Dynamics.RemoteInputSignal
        
          PFVArControllerType1Dynamics --> RemoteInputSignal : PFVArControllerType1Dynamics.RemoteInputSignal
        
      PFVArControllerType1Dynamics : PFVArControllerType1Dynamics.VoltageAdjusterDynamics
        
          PFVArControllerType1Dynamics --> VoltageAdjusterDynamics : PFVArControllerType1Dynamics.VoltageAdjusterDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **PFVArControllerType1Dynamics**
            * [PFVArControllerType1UserDefined](PFVArControllerType1UserDefined.md)
            * [PFVArType1IEEEPFController](PFVArType1IEEEPFController.md)
            * [PFVArType1IEEEVArController](PFVArType1IEEEVArController.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RemoteInputSignal | [cim:PFVArControllerType1Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this power factor or VAr controller type 1 model | direct |
| ExcitationSystemDynamics | [cim:PFVArControllerType1Dynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power actor or VAr controller type 1 ... | direct |
| VoltageAdjusterDynamics | [cim:PFVArControllerType1Dynamics.VoltageAdjusterDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.VoltageAdjusterDynamics) | 0..1 <br />  [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md)  | Voltage adjuster model associated with this power factor or VAr controller ty... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RemoteInputSignal](RemoteInputSignal.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcitationSystemUserDefined](ExcitationSystemUserDefined.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [VoltageAdjusterUserDefined](VoltageAdjusterUserDefined.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcitationSystemDynamics](ExcitationSystemDynamics.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC1A](ExcIEEEAC1A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC2A](ExcIEEEAC2A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC3A](ExcIEEEAC3A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC4A](ExcIEEEAC4A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC5A](ExcIEEEAC5A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC6A](ExcIEEEAC6A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC7B](ExcIEEEAC7B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEAC8B](ExcIEEEAC8B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEDC1A](ExcIEEEDC1A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEDC2A](ExcIEEEDC2A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEDC3A](ExcIEEEDC3A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEDC4B](ExcIEEEDC4B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST1A](ExcIEEEST1A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST2A](ExcIEEEST2A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST3A](ExcIEEEST3A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST4B](ExcIEEEST4B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST5B](ExcIEEEST5B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST6B](ExcIEEEST6B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcIEEEST7B](ExcIEEEST7B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC1A](ExcAC1A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC2A](ExcAC2A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC3A](ExcAC3A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC4A](ExcAC4A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC5A](ExcAC5A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC6A](ExcAC6A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAC8B](ExcAC8B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcANS](ExcANS.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAVR1](ExcAVR1.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAVR2](ExcAVR2.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAVR3](ExcAVR3.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAVR4](ExcAVR4.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAVR5](ExcAVR5.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcAVR7](ExcAVR7.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcBBC](ExcBBC.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcCZ](ExcCZ.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcDC1A](ExcDC1A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcDC2A](ExcDC2A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcDC3A](ExcDC3A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcDC3A1](ExcDC3A1.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcELIN1](ExcELIN1.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcELIN2](ExcELIN2.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcHU](ExcHU.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcNI](ExcNI.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcOEX3T](ExcOEX3T.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcPIC](ExcPIC.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcREXS](ExcREXS.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcRQB](ExcRQB.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcSCRX](ExcSCRX.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcSEXS](ExcSEXS.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcSK](ExcSK.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcST1A](ExcST1A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcST2A](ExcST2A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcST3A](ExcST3A.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcST4B](ExcST4B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcST6B](ExcST6B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [ExcST7B](ExcST7B.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| [VAdjIEEE](VAdjIEEE.md) | PFVArControllerType1Dynamics | range | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PFVArControllerType1Dynamics |
| native | this:PFVArControllerType1Dynamics |




