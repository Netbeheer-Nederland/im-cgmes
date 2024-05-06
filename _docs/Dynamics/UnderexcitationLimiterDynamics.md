# UnderexcitationLimiterDynamics


_Underexcitation limiter function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:UnderexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class UnderexcitationLimiterDynamics
    click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
      DynamicsFunctionBlock <|-- UnderexcitationLimiterDynamics
        click DynamicsFunctionBlock href "../DynamicsFunctionBlock"
      

      UnderexcitationLimiterDynamics <|-- UnderexcitationLimiterUserDefined
        click UnderexcitationLimiterUserDefined href "../UnderexcitationLimiterUserDefined"
      UnderexcitationLimiterDynamics <|-- UnderexcLimIEEE1
        click UnderexcLimIEEE1 href "../UnderexcLimIEEE1"
      UnderexcitationLimiterDynamics <|-- UnderexcLimIEEE2
        click UnderexcLimIEEE2 href "../UnderexcLimIEEE2"
      UnderexcitationLimiterDynamics <|-- UnderexcLim2Simplified
        click UnderexcLim2Simplified href "../UnderexcLim2Simplified"
      UnderexcitationLimiterDynamics <|-- UnderexcLimX1
        click UnderexcLimX1 href "../UnderexcLimX1"
      UnderexcitationLimiterDynamics <|-- UnderexcLimX2
        click UnderexcLimX2 href "../UnderexcLimX2"
      
      
      UnderexcitationLimiterDynamics : IdentifiedObject.description
        
      UnderexcitationLimiterDynamics : DynamicsFunctionBlock.enabled
        
      UnderexcitationLimiterDynamics : UnderexcitationLimiterDynamics.ExcitationSystemDynamics
        
          UnderexcitationLimiterDynamics --> ExcitationSystemDynamics : UnderexcitationLimiterDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      UnderexcitationLimiterDynamics : IdentifiedObject.mRID
        
      UnderexcitationLimiterDynamics : IdentifiedObject.name
        
      UnderexcitationLimiterDynamics : UnderexcitationLimiterDynamics.RemoteInputSignal
        
          UnderexcitationLimiterDynamics --> RemoteInputSignal : UnderexcitationLimiterDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **UnderexcitationLimiterDynamics**
            * [UnderexcitationLimiterUserDefined](UnderexcitationLimiterUserDefined.md)
            * [UnderexcLimIEEE1](UnderexcLimIEEE1.md)
            * [UnderexcLimIEEE2](UnderexcLimIEEE2.md)
            * [UnderexcLim2Simplified](UnderexcLim2Simplified.md)
            * [UnderexcLimX1](UnderexcLimX1.md)
            * [UnderexcLimX2](UnderexcLimX2.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RemoteInputSignal | [cim:UnderexcitationLimiterDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this underexcitation limiter model | direct |
| ExcitationSystemDynamics | [cim:UnderexcitationLimiterDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this underexcitation limiter model is asso... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RemoteInputSignal](RemoteInputSignal.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcitationSystemUserDefined](ExcitationSystemUserDefined.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcitationSystemDynamics](ExcitationSystemDynamics.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC1A](ExcIEEEAC1A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC2A](ExcIEEEAC2A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC3A](ExcIEEEAC3A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC4A](ExcIEEEAC4A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC5A](ExcIEEEAC5A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC6A](ExcIEEEAC6A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC7B](ExcIEEEAC7B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEAC8B](ExcIEEEAC8B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEDC1A](ExcIEEEDC1A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEDC2A](ExcIEEEDC2A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEDC3A](ExcIEEEDC3A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEDC4B](ExcIEEEDC4B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST1A](ExcIEEEST1A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST2A](ExcIEEEST2A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST3A](ExcIEEEST3A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST4B](ExcIEEEST4B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST5B](ExcIEEEST5B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST6B](ExcIEEEST6B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcIEEEST7B](ExcIEEEST7B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC1A](ExcAC1A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC2A](ExcAC2A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC3A](ExcAC3A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC4A](ExcAC4A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC5A](ExcAC5A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC6A](ExcAC6A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAC8B](ExcAC8B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcANS](ExcANS.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAVR1](ExcAVR1.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAVR2](ExcAVR2.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAVR3](ExcAVR3.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAVR4](ExcAVR4.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAVR5](ExcAVR5.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcAVR7](ExcAVR7.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcBBC](ExcBBC.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcCZ](ExcCZ.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcDC1A](ExcDC1A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcDC2A](ExcDC2A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcDC3A](ExcDC3A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcDC3A1](ExcDC3A1.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcELIN1](ExcELIN1.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcELIN2](ExcELIN2.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcHU](ExcHU.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcNI](ExcNI.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcOEX3T](ExcOEX3T.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcPIC](ExcPIC.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcREXS](ExcREXS.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcRQB](ExcRQB.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcSCRX](ExcSCRX.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcSEXS](ExcSEXS.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcSK](ExcSK.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcST1A](ExcST1A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcST2A](ExcST2A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcST3A](ExcST3A.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcST4B](ExcST4B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcST6B](ExcST6B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| [ExcST7B](ExcST7B.md) | UnderexcitationLimiterDynamics | range | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:UnderexcitationLimiterDynamics |
| native | this:UnderexcitationLimiterDynamics |




