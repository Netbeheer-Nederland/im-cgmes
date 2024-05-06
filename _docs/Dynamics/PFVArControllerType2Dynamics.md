# PFVArControllerType2Dynamics


_Power factor or VAr controller type 2 function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:PFVArControllerType2Dynamics](http://iec.ch/TC57/CIM100#PFVArControllerType2Dynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class PFVArControllerType2Dynamics
    click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
      DynamicsFunctionBlock <|-- PFVArControllerType2Dynamics
        click DynamicsFunctionBlock href "../DynamicsFunctionBlock"
      

      PFVArControllerType2Dynamics <|-- PFVArControllerType2UserDefined
        click PFVArControllerType2UserDefined href "../PFVArControllerType2UserDefined"
      PFVArControllerType2Dynamics <|-- PFVArType2IEEEPFController
        click PFVArType2IEEEPFController href "../PFVArType2IEEEPFController"
      PFVArControllerType2Dynamics <|-- PFVArType2IEEEVArController
        click PFVArType2IEEEVArController href "../PFVArType2IEEEVArController"
      PFVArControllerType2Dynamics <|-- PFVArType2Common1
        click PFVArType2Common1 href "../PFVArType2Common1"
      
      
      PFVArControllerType2Dynamics : IdentifiedObject.description
        
      PFVArControllerType2Dynamics : DynamicsFunctionBlock.enabled
        
      PFVArControllerType2Dynamics : PFVArControllerType2Dynamics.ExcitationSystemDynamics
        
          PFVArControllerType2Dynamics --> ExcitationSystemDynamics : PFVArControllerType2Dynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      PFVArControllerType2Dynamics : IdentifiedObject.mRID
        
      PFVArControllerType2Dynamics : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **PFVArControllerType2Dynamics**
            * [PFVArControllerType2UserDefined](PFVArControllerType2UserDefined.md)
            * [PFVArType2IEEEPFController](PFVArType2IEEEPFController.md)
            * [PFVArType2IEEEVArController](PFVArType2IEEEVArController.md)
            * [PFVArType2Common1](PFVArType2Common1.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ExcitationSystemDynamics | [cim:PFVArControllerType2Dynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType2Dynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power factor or VAr controller type 2... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ExcitationSystemUserDefined](ExcitationSystemUserDefined.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcitationSystemDynamics](ExcitationSystemDynamics.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC1A](ExcIEEEAC1A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC2A](ExcIEEEAC2A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC3A](ExcIEEEAC3A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC4A](ExcIEEEAC4A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC5A](ExcIEEEAC5A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC6A](ExcIEEEAC6A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC7B](ExcIEEEAC7B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEAC8B](ExcIEEEAC8B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEDC1A](ExcIEEEDC1A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEDC2A](ExcIEEEDC2A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEDC3A](ExcIEEEDC3A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEDC4B](ExcIEEEDC4B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST1A](ExcIEEEST1A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST2A](ExcIEEEST2A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST3A](ExcIEEEST3A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST4B](ExcIEEEST4B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST5B](ExcIEEEST5B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST6B](ExcIEEEST6B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcIEEEST7B](ExcIEEEST7B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC1A](ExcAC1A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC2A](ExcAC2A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC3A](ExcAC3A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC4A](ExcAC4A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC5A](ExcAC5A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC6A](ExcAC6A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAC8B](ExcAC8B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcANS](ExcANS.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAVR1](ExcAVR1.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAVR2](ExcAVR2.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAVR3](ExcAVR3.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAVR4](ExcAVR4.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAVR5](ExcAVR5.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcAVR7](ExcAVR7.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcBBC](ExcBBC.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcCZ](ExcCZ.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcDC1A](ExcDC1A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcDC2A](ExcDC2A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcDC3A](ExcDC3A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcDC3A1](ExcDC3A1.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcELIN1](ExcELIN1.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcELIN2](ExcELIN2.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcHU](ExcHU.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcNI](ExcNI.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcOEX3T](ExcOEX3T.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcPIC](ExcPIC.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcREXS](ExcREXS.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcRQB](ExcRQB.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcSCRX](ExcSCRX.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcSEXS](ExcSEXS.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcSK](ExcSK.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcST1A](ExcST1A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcST2A](ExcST2A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcST3A](ExcST3A.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcST4B](ExcST4B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcST6B](ExcST6B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| [ExcST7B](ExcST7B.md) | PFVArControllerType2Dynamics | range | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PFVArControllerType2Dynamics |
| native | this:PFVArControllerType2Dynamics |




