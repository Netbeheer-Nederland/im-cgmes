# ExcAVR2


_Italian excitation system corresponding to IEEE (1968) type 2 model. It represents an alternator and rotating diodes and electromechanic voltage regulators._





**URI**: [cim:ExcAVR2](http://iec.ch/TC57/CIM100#ExcAVR2)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAVR2
    click ExcAVR2 href "../ExcAVR2"
      ExcitationSystemDynamics <|-- ExcAVR2
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcAVR2 : IdentifiedObject.description
        
      ExcAVR2 : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAVR2 --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcAVR2 : ExcAVR2.e1
        
          ExcAVR2 --> PU : ExcAVR2.e1
          click PU href "../PU"
        
      ExcAVR2 : ExcAVR2.e2
        
          ExcAVR2 --> PU : ExcAVR2.e2
          click PU href "../PU"
        
      ExcAVR2 : DynamicsFunctionBlock.enabled
        
      ExcAVR2 : ExcAVR2.ka
        
      ExcAVR2 : ExcAVR2.kf
        
      ExcAVR2 : IdentifiedObject.mRID
        
      ExcAVR2 : IdentifiedObject.name
        
      ExcAVR2 : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAVR2 --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcAVR2 : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAVR2 --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcAVR2 : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAVR2 --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcAVR2 : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAVR2 --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcAVR2 : ExcAVR2.se1
        
      ExcAVR2 : ExcAVR2.se2
        
      ExcAVR2 : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAVR2 --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcAVR2 : ExcAVR2.ta
        
          ExcAVR2 --> Seconds : ExcAVR2.ta
          click Seconds href "../Seconds"
        
      ExcAVR2 : ExcAVR2.tb
        
          ExcAVR2 --> Seconds : ExcAVR2.tb
          click Seconds href "../Seconds"
        
      ExcAVR2 : ExcAVR2.te
        
          ExcAVR2 --> Seconds : ExcAVR2.te
          click Seconds href "../Seconds"
        
      ExcAVR2 : ExcAVR2.tf1
        
          ExcAVR2 --> Seconds : ExcAVR2.tf1
          click Seconds href "../Seconds"
        
      ExcAVR2 : ExcAVR2.tf2
        
          ExcAVR2 --> Seconds : ExcAVR2.tf2
          click Seconds href "../Seconds"
        
      ExcAVR2 : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAVR2 --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcAVR2 : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAVR2 --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcAVR2 : ExcAVR2.vrmn
        
          ExcAVR2 --> PU : ExcAVR2.vrmn
          click PU href "../PU"
        
      ExcAVR2 : ExcAVR2.vrmx
        
          ExcAVR2 --> PU : ExcAVR2.vrmx
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAVR2**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcAVR2.ka](http://iec.ch/TC57/CIM100#ExcAVR2.ka) | 1 <br />  float  | AVR gain (<i>K</i><i><sub>A</sub></i>) | direct |
| vrmn | [cim:ExcAVR2.vrmn](http://iec.ch/TC57/CIM100#ExcAVR2.vrmn) | 1 <br />  [PU](PU.md)  | Minimum AVR output (<i>V</i><i><sub>RMN</sub></i>) | direct |
| vrmx | [cim:ExcAVR2.vrmx](http://iec.ch/TC57/CIM100#ExcAVR2.vrmx) | 1 <br />  [PU](PU.md)  | Maximum AVR output (<i>V</i><i><sub>RMX</sub></i>) | direct |
| ta | [cim:ExcAVR2.ta](http://iec.ch/TC57/CIM100#ExcAVR2.ta) | 1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>A</sub></i>) (&gt;= 0) | direct |
| tb | [cim:ExcAVR2.tb](http://iec.ch/TC57/CIM100#ExcAVR2.tb) | 1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>B</sub></i>) (&gt;= 0) | direct |
| te | [cim:ExcAVR2.te](http://iec.ch/TC57/CIM100#ExcAVR2.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant (<i>T</i><i><sub>E</sub></i>) (&gt;= 0) | direct |
| e1 | [cim:ExcAVR2.e1](http://iec.ch/TC57/CIM100#ExcAVR2.e1) | 1 <br />  [PU](PU.md)  | Field voltage value 1 (<i>E</i><i><sub>1</sub></i>) | direct |
| se1 | [cim:ExcAVR2.se1](http://iec.ch/TC57/CIM100#ExcAVR2.se1) | 1 <br />  float  | Saturation factor at <i>E</i><i><sub>1</sub></i> (<i>S[E</i><i><sub>1</sub></... | direct |
| e2 | [cim:ExcAVR2.e2](http://iec.ch/TC57/CIM100#ExcAVR2.e2) | 1 <br />  [PU](PU.md)  | Field voltage value 2 (<i>E</i><i><sub>2</sub></i>) | direct |
| se2 | [cim:ExcAVR2.se2](http://iec.ch/TC57/CIM100#ExcAVR2.se2) | 1 <br />  float  | Saturation factor at <i>E</i><i><sub>2</sub></i> (<i>S[E</i><i><sub>2</sub></... | direct |
| kf | [cim:ExcAVR2.kf](http://iec.ch/TC57/CIM100#ExcAVR2.kf) | 1 <br />  float  | Rate feedback gain (<i>K</i><i><sub>F</sub></i>) | direct |
| tf1 | [cim:ExcAVR2.tf1](http://iec.ch/TC57/CIM100#ExcAVR2.tf1) | 1 <br />  [Seconds](Seconds.md)  | Rate feedback time constant (<i>T</i><i><sub>F1</sub></i>) (&gt;= 0) | direct |
| tf2 | [cim:ExcAVR2.tf2](http://iec.ch/TC57/CIM100#ExcAVR2.tf2) | 1 <br />  [Seconds](Seconds.md)  | Rate feedback time constant (<i>T</i><i><sub>F2</sub></i>) (&gt;= 0) | direct |
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
| self | cim:ExcAVR2 |
| native | this:ExcAVR2 |




