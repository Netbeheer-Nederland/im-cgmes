# ExcAVR1


_Italian excitation system corresponding to IEEE (1968) type 1 model. It represents an exciter dynamo and electromechanical regulator._





**URI**: [cim:ExcAVR1](http://iec.ch/TC57/CIM100#ExcAVR1)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAVR1
      ExcitationSystemDynamics <|-- ExcAVR1
      
      ExcAVR1 : IdentifiedObject.description
        
      ExcAVR1 : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAVR1 --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcAVR1 : ExcAVR1.e1
        
          ExcAVR1 --> PU : ExcAVR1.e1
        
      ExcAVR1 : ExcAVR1.e2
        
          ExcAVR1 --> PU : ExcAVR1.e2
        
      ExcAVR1 : DynamicsFunctionBlock.enabled
        
      ExcAVR1 : ExcAVR1.ka
        
      ExcAVR1 : ExcAVR1.kf
        
      ExcAVR1 : IdentifiedObject.mRID
        
      ExcAVR1 : IdentifiedObject.name
        
      ExcAVR1 : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAVR1 --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcAVR1 : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAVR1 --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcAVR1 : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAVR1 --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcAVR1 : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAVR1 --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcAVR1 : ExcAVR1.se1
        
      ExcAVR1 : ExcAVR1.se2
        
      ExcAVR1 : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAVR1 --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcAVR1 : ExcAVR1.ta
        
          ExcAVR1 --> Seconds : ExcAVR1.ta
        
      ExcAVR1 : ExcAVR1.tb
        
          ExcAVR1 --> Seconds : ExcAVR1.tb
        
      ExcAVR1 : ExcAVR1.te
        
          ExcAVR1 --> Seconds : ExcAVR1.te
        
      ExcAVR1 : ExcAVR1.tf
        
          ExcAVR1 --> Seconds : ExcAVR1.tf
        
      ExcAVR1 : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAVR1 --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcAVR1 : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAVR1 --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcAVR1 : ExcAVR1.vrmn
        
          ExcAVR1 --> PU : ExcAVR1.vrmn
        
      ExcAVR1 : ExcAVR1.vrmx
        
          ExcAVR1 --> PU : ExcAVR1.vrmx
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAVR1**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcAVR1.ka](http://iec.ch/TC57/CIM100#ExcAVR1.ka) | 1..1 <br />  float  | AVR gain (<i>K</i><i><sub>A</sub></i>) | direct |
| vrmn | [cim:ExcAVR1.vrmn](http://iec.ch/TC57/CIM100#ExcAVR1.vrmn) | 1..1 <br />  [PU](PU.md)  | Minimum AVR output (<i>V</i><i><sub>RMN</sub></i>) | direct |
| vrmx | [cim:ExcAVR1.vrmx](http://iec.ch/TC57/CIM100#ExcAVR1.vrmx) | 1..1 <br />  [PU](PU.md)  | Maximum AVR output (<i>V</i><i><sub>RMX</sub></i>) | direct |
| ta | [cim:ExcAVR1.ta](http://iec.ch/TC57/CIM100#ExcAVR1.ta) | 1..1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>A</sub></i>) (&gt;= 0) | direct |
| tb | [cim:ExcAVR1.tb](http://iec.ch/TC57/CIM100#ExcAVR1.tb) | 1..1 <br />  [Seconds](Seconds.md)  | AVR time constant (<i>T</i><i><sub>B</sub></i>) (&gt;= 0) | direct |
| te | [cim:ExcAVR1.te](http://iec.ch/TC57/CIM100#ExcAVR1.te) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter time constant (<i>T</i><i><sub>E</sub></i>) (&gt;= 0) | direct |
| e1 | [cim:ExcAVR1.e1](http://iec.ch/TC57/CIM100#ExcAVR1.e1) | 1..1 <br />  [PU](PU.md)  | Field voltage value 1 (<i>E</i><i><sub>1</sub></i>) | direct |
| se1 | [cim:ExcAVR1.se1](http://iec.ch/TC57/CIM100#ExcAVR1.se1) | 1..1 <br />  float  | Saturation factor at <i>E</i><i><sub>1</sub></i> (<i>S[E</i><i><sub>1</sub></... | direct |
| e2 | [cim:ExcAVR1.e2](http://iec.ch/TC57/CIM100#ExcAVR1.e2) | 1..1 <br />  [PU](PU.md)  | Field voltage value 2 (<i>E</i><i><sub>2</sub></i>) | direct |
| se2 | [cim:ExcAVR1.se2](http://iec.ch/TC57/CIM100#ExcAVR1.se2) | 1..1 <br />  float  | Saturation factor at <i>E</i><i><sub>2</sub></i> (<i>S[E</i><i><sub>2</sub></... | direct |
| kf | [cim:ExcAVR1.kf](http://iec.ch/TC57/CIM100#ExcAVR1.kf) | 1..1 <br />  float  | Rate feedback gain (<i>K</i><i><sub>F</sub></i>) | direct |
| tf | [cim:ExcAVR1.tf](http://iec.ch/TC57/CIM100#ExcAVR1.tf) | 1..1 <br />  [Seconds](Seconds.md)  | Rate feedback time constant (<i>T</i><i><sub>F</sub></i>) (&gt;= 0) | direct |
| SynchronousMachineDynamics | [cim:ExcitationSystemDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.SynchronousMachineDynamics) | 1..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this excitation system model is associat... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| VoltageCompensatorDynamics | [cim:ExcitationSystemDynamics.VoltageCompensatorDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.VoltageCompensatorDynamics) | 1..1 <br />  [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)  | Voltage compensator model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| OverexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.OverexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.OverexcitationLimiterDynamics) | 0..1 <br />  [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md)  | Overexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType2Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType2Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType2Dynamics) | 0..1 <br />  [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md)  | Power factor or VAr controller type 2 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| DiscontinuousExcitationControlDynamics | [cim:ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics) | 0..1 <br />  [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md)  | Discontinuous excitation control model associated with this excitation system... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PowerSystemStabilizerDynamics | [cim:ExcitationSystemDynamics.PowerSystemStabilizerDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PowerSystemStabilizerDynamics) | 0..1 <br />  [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)  | Power system stabilizer model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| UnderexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.UnderexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.UnderexcitationLimiterDynamics) | 0..1 <br />  [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md)  | Undrexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType1Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType1Dynamics) | 0..1 <br />  [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)  | Power factor or VAr controller type 1 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ExcAVR1 |
| native | this:ExcAVR1 |




