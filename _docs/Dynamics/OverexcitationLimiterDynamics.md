# OverexcitationLimiterDynamics


_Overexcitation limiter function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:OverexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#OverexcitationLimiterDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class OverexcitationLimiterDynamics
      DynamicsFunctionBlock <|-- OverexcitationLimiterDynamics
      

      OverexcitationLimiterDynamics <|-- OverexcitationLimiterUserDefined
      OverexcitationLimiterDynamics <|-- OverexcLimIEEE
      OverexcitationLimiterDynamics <|-- OverexcLim2
      OverexcitationLimiterDynamics <|-- OverexcLimX1
      OverexcitationLimiterDynamics <|-- OverexcLimX2
      
      
      OverexcitationLimiterDynamics : IdentifiedObject.description
        
      OverexcitationLimiterDynamics : DynamicsFunctionBlock.enabled
        
      OverexcitationLimiterDynamics : OverexcitationLimiterDynamics.ExcitationSystemDynamics
        
          OverexcitationLimiterDynamics --> ExcitationSystemDynamics : OverexcitationLimiterDynamics.ExcitationSystemDynamics
        
      OverexcitationLimiterDynamics : IdentifiedObject.mRID
        
      OverexcitationLimiterDynamics : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **OverexcitationLimiterDynamics**
            * [OverexcitationLimiterUserDefined](OverexcitationLimiterUserDefined.md)
            * [OverexcLimIEEE](OverexcLimIEEE.md)
            * [OverexcLim2](OverexcLim2.md)
            * [OverexcLimX1](OverexcLimX1.md)
            * [OverexcLimX2](OverexcLimX2.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ExcitationSystemDynamics | [cim:OverexcitationLimiterDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#OverexcitationLimiterDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this overexcitation limiter model is assoc... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ExcitationSystemUserDefined](ExcitationSystemUserDefined.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcitationSystemDynamics](ExcitationSystemDynamics.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC1A](ExcIEEEAC1A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC2A](ExcIEEEAC2A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC3A](ExcIEEEAC3A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC4A](ExcIEEEAC4A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC5A](ExcIEEEAC5A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC6A](ExcIEEEAC6A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC7B](ExcIEEEAC7B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEAC8B](ExcIEEEAC8B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEDC1A](ExcIEEEDC1A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEDC2A](ExcIEEEDC2A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEDC3A](ExcIEEEDC3A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEDC4B](ExcIEEEDC4B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST1A](ExcIEEEST1A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST2A](ExcIEEEST2A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST3A](ExcIEEEST3A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST4B](ExcIEEEST4B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST5B](ExcIEEEST5B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST6B](ExcIEEEST6B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcIEEEST7B](ExcIEEEST7B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC1A](ExcAC1A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC2A](ExcAC2A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC3A](ExcAC3A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC4A](ExcAC4A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC5A](ExcAC5A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC6A](ExcAC6A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAC8B](ExcAC8B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcANS](ExcANS.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAVR1](ExcAVR1.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAVR2](ExcAVR2.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAVR3](ExcAVR3.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAVR4](ExcAVR4.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAVR5](ExcAVR5.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcAVR7](ExcAVR7.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcBBC](ExcBBC.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcCZ](ExcCZ.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcDC1A](ExcDC1A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcDC2A](ExcDC2A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcDC3A](ExcDC3A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcDC3A1](ExcDC3A1.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcELIN1](ExcELIN1.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcELIN2](ExcELIN2.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcHU](ExcHU.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcNI](ExcNI.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcOEX3T](ExcOEX3T.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcPIC](ExcPIC.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcREXS](ExcREXS.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcRQB](ExcRQB.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcSCRX](ExcSCRX.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcSEXS](ExcSEXS.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcSK](ExcSK.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcST1A](ExcST1A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcST2A](ExcST2A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcST3A](ExcST3A.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcST4B](ExcST4B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcST6B](ExcST6B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| [ExcST7B](ExcST7B.md) | OverexcitationLimiterDynamics | range | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:OverexcitationLimiterDynamics |
| native | this:OverexcitationLimiterDynamics |




