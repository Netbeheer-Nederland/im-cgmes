# UnderexcLimX1


_<font color="#0f0f0f">Allis-Chalmers minimum excitation limiter.</font>_





**URI**: [cim:UnderexcLimX1](http://iec.ch/TC57/CIM100#UnderexcLimX1)<br />
**Type**: Class




```mermaid
 classDiagram
    class UnderexcLimX1
    click UnderexcLimX1 href "../UnderexcLimX1"
      UnderexcitationLimiterDynamics <|-- UnderexcLimX1
        click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
      
      UnderexcLimX1 : IdentifiedObject.description
        
      UnderexcLimX1 : DynamicsFunctionBlock.enabled
        
      UnderexcLimX1 : UnderexcitationLimiterDynamics.ExcitationSystemDynamics
        
          UnderexcLimX1 --> ExcitationSystemDynamics : UnderexcitationLimiterDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      UnderexcLimX1 : UnderexcLimX1.k
        
          UnderexcLimX1 --> PU : UnderexcLimX1.k
          click PU href "../PU"
        
      UnderexcLimX1 : UnderexcLimX1.kf2
        
          UnderexcLimX1 --> PU : UnderexcLimX1.kf2
          click PU href "../PU"
        
      UnderexcLimX1 : UnderexcLimX1.km
        
          UnderexcLimX1 --> PU : UnderexcLimX1.km
          click PU href "../PU"
        
      UnderexcLimX1 : UnderexcLimX1.melmax
        
          UnderexcLimX1 --> PU : UnderexcLimX1.melmax
          click PU href "../PU"
        
      UnderexcLimX1 : IdentifiedObject.mRID
        
      UnderexcLimX1 : IdentifiedObject.name
        
      UnderexcLimX1 : UnderexcitationLimiterDynamics.RemoteInputSignal
        
          UnderexcLimX1 --> RemoteInputSignal : UnderexcitationLimiterDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      UnderexcLimX1 : UnderexcLimX1.tf2
        
          UnderexcLimX1 --> Seconds : UnderexcLimX1.tf2
          click Seconds href "../Seconds"
        
      UnderexcLimX1 : UnderexcLimX1.tm
        
          UnderexcLimX1 --> Seconds : UnderexcLimX1.tm
          click Seconds href "../Seconds"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md)
            * **UnderexcLimX1**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| kf2 | [cim:UnderexcLimX1.kf2](http://iec.ch/TC57/CIM100#UnderexcLimX1.kf2) | 1 <br />  [PU](PU.md)  | Differential gain (<i>K</i><i><sub>F2</sub></i>) | direct |
| tf2 | [cim:UnderexcLimX1.tf2](http://iec.ch/TC57/CIM100#UnderexcLimX1.tf2) | 1 <br />  [Seconds](Seconds.md)  | Differential time constant (<i>T</i><i><sub>F2</sub></i>) (&gt;= 0) | direct |
| km | [cim:UnderexcLimX1.km](http://iec.ch/TC57/CIM100#UnderexcLimX1.km) | 1 <br />  [PU](PU.md)  | Minimum excitation limit gain (<i>K</i><i><sub>M</sub></i>) | direct |
| tm | [cim:UnderexcLimX1.tm](http://iec.ch/TC57/CIM100#UnderexcLimX1.tm) | 1 <br />  [Seconds](Seconds.md)  | Minimum excitation limit time constant (<i>T</i><i><sub>M</sub></i>) (&gt;= 0... | direct |
| melmax | [cim:UnderexcLimX1.melmax](http://iec.ch/TC57/CIM100#UnderexcLimX1.melmax) | 1 <br />  [PU](PU.md)  | Minimum excitation limit value (<i>MELMAX</i>) | direct |
| k | [cim:UnderexcLimX1.k](http://iec.ch/TC57/CIM100#UnderexcLimX1.k) | 1 <br />  [PU](PU.md)  | Minimum excitation limit slope (<i>K</i>) (&gt; 0) | direct |
| RemoteInputSignal | [cim:UnderexcitationLimiterDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this underexcitation limiter model | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| ExcitationSystemDynamics | [cim:UnderexcitationLimiterDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this underexcitation limiter model is asso... | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
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
| self | cim:UnderexcLimX1 |
| native | this:UnderexcLimX1 |




