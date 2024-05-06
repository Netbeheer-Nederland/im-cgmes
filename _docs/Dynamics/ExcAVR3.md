# ExcAVR3


_Italian excitation system. It represents an exciter dynamo and electric regulator._





**URI**: [cim:ExcAVR3](http://iec.ch/TC57/CIM100#ExcAVR3)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAVR3
    click ExcAVR3 href "../ExcAVR3"
      ExcitationSystemDynamics <|-- ExcAVR3
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcAVR3 : IdentifiedObject.description
        
      ExcAVR3 : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAVR3 --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcAVR3 : ExcAVR3.e1
        
          ExcAVR3 --> PU : ExcAVR3.e1
          click PU href "../PU"
        
      ExcAVR3 : ExcAVR3.e2
        
          ExcAVR3 --> PU : ExcAVR3.e2
          click PU href "../PU"
        
      ExcAVR3 : DynamicsFunctionBlock.enabled
        
      ExcAVR3 : ExcAVR3.ka
        
      ExcAVR3 : IdentifiedObject.mRID
        
      ExcAVR3 : IdentifiedObject.name
        
      ExcAVR3 : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAVR3 --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcAVR3 : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAVR3 --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcAVR3 : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAVR3 --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcAVR3 : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAVR3 --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcAVR3 : ExcAVR3.se1
        
      ExcAVR3 : ExcAVR3.se2
        
      ExcAVR3 : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAVR3 --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcAVR3 : ExcAVR3.t1
        
          ExcAVR3 --> Seconds : ExcAVR3.t1
          click Seconds href "../Seconds"
        
      ExcAVR3 : ExcAVR3.t2
        
          ExcAVR3 --> Seconds : ExcAVR3.t2
          click Seconds href "../Seconds"
        
      ExcAVR3 : ExcAVR3.t3
        
          ExcAVR3 --> Seconds : ExcAVR3.t3
          click Seconds href "../Seconds"
        
      ExcAVR3 : ExcAVR3.t4
        
          ExcAVR3 --> Seconds : ExcAVR3.t4
          click Seconds href "../Seconds"
        
      ExcAVR3 : ExcAVR3.te
        
          ExcAVR3 --> Seconds : ExcAVR3.te
          click Seconds href "../Seconds"
        
      ExcAVR3 : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAVR3 --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcAVR3 : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAVR3 --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcAVR3 : ExcAVR3.vrmn
        
          ExcAVR3 --> PU : ExcAVR3.vrmn
          click PU href "../PU"
        
      ExcAVR3 : ExcAVR3.vrmx
        
          ExcAVR3 --> PU : ExcAVR3.vrmx
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAVR3**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcAVR3.ka](http://iec.ch/TC57/CIM100#ExcAVR3.ka) | 1 <br />  float  | AVR gain (<i>K</i><i><sub>A</sub></i>) | direct |
| vrmn | [cim:ExcAVR3.vrmn](http://iec.ch/TC57/CIM100#ExcAVR3.vrmn) | 1 <br />  [PU](PU.md)  | Minimum AVR output (<i>V</i><i><sub>RMN</sub></i>) | direct |
| vrmx | [cim:ExcAVR3.vrmx](http://iec.ch/TC57/CIM100#ExcAVR3.vrmx) | 1 <br />  [PU](PU.md)  | Maximum AVR output (<i>V</i><i><sub>RMX</sub></i>) | direct |
| t1 | [cim:ExcAVR3.t1](http://iec.ch/TC57/CIM100#ExcAVR3.t1) | 1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>1</sub></i>) (&gt;= 0) | direct |
| t2 | [cim:ExcAVR3.t2](http://iec.ch/TC57/CIM100#ExcAVR3.t2) | 1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>2</sub></i>) (&gt;= 0) | direct |
| t3 | [cim:ExcAVR3.t3](http://iec.ch/TC57/CIM100#ExcAVR3.t3) | 1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>3</sub></i>) (&gt;= 0) | direct |
| t4 | [cim:ExcAVR3.t4](http://iec.ch/TC57/CIM100#ExcAVR3.t4) | 1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>4</sub></i>) (&gt;= 0) | direct |
| te | [cim:ExcAVR3.te](http://iec.ch/TC57/CIM100#ExcAVR3.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant (<i>T</i><i><sub>E</sub></i>) (&gt;= 0) | direct |
| e1 | [cim:ExcAVR3.e1](http://iec.ch/TC57/CIM100#ExcAVR3.e1) | 1 <br />  [PU](PU.md)  | Field voltage value 1 (<i>E</i><i><sub>1</sub></i>) | direct |
| se1 | [cim:ExcAVR3.se1](http://iec.ch/TC57/CIM100#ExcAVR3.se1) | 1 <br />  float  | Saturation factor at <i>E</i><i><sub>1</sub></i><i> </i>(<i>S[E</i><i><sub>1<... | direct |
| e2 | [cim:ExcAVR3.e2](http://iec.ch/TC57/CIM100#ExcAVR3.e2) | 1 <br />  [PU](PU.md)  | Field voltage value 2 (<i>E</i><i><sub>2</sub></i>) | direct |
| se2 | [cim:ExcAVR3.se2](http://iec.ch/TC57/CIM100#ExcAVR3.se2) | 1 <br />  float  | Saturation factor at <i>E</i><i><sub>2</sub></i><i> </i>(<i>S[E</i><i><sub>2<... | direct |
| SynchronousMachineDynamics | [cim:ExcitationSystemDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.SynchronousMachineDynamics) | 1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this excitation system model is associat... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| VoltageCompensatorDynamics | [cim:ExcitationSystemDynamics.VoltageCompensatorDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.VoltageCompensatorDynamics) | 1 <br />  [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)  | Voltage compensator model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| OverexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.OverexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.OverexcitationLimiterDynamics) | 0..1 <br />  [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md)  | Overexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType2Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType2Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType2Dynamics) | 0..1 <br />  [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md)  | Power factor or VAr controller type 2 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| DiscontinuousExcitationControlDynamics | [cim:ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics) | 0..1 <br />  [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md)  | Discontinuous excitation control model associated with this excitation system... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PowerSystemStabilizerDynamics | [cim:ExcitationSystemDynamics.PowerSystemStabilizerDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PowerSystemStabilizerDynamics) | 0..1 <br />  [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)  | Power system stabilizer model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| UnderexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.UnderexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.UnderexcitationLimiterDynamics) | 0..1 <br />  [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md)  | Undrexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType1Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType1Dynamics) | 0..1 <br />  [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)  | Power factor or VAr controller type 1 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
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
| self | cim:ExcAVR3 |
| native | this:ExcAVR3 |




