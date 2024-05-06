# ExcCZ


_Czech proportion/integral exciter._





**URI**: [cim:ExcCZ](http://iec.ch/TC57/CIM100#ExcCZ)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcCZ
    click ExcCZ href "../ExcCZ"
      ExcitationSystemDynamics <|-- ExcCZ
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcCZ : IdentifiedObject.description
        
      ExcCZ : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcCZ --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcCZ : ExcCZ.efdmax
        
          ExcCZ --> PU : ExcCZ.efdmax
          click PU href "../PU"
        
      ExcCZ : ExcCZ.efdmin
        
          ExcCZ --> PU : ExcCZ.efdmin
          click PU href "../PU"
        
      ExcCZ : DynamicsFunctionBlock.enabled
        
      ExcCZ : ExcCZ.ka
        
          ExcCZ --> PU : ExcCZ.ka
          click PU href "../PU"
        
      ExcCZ : ExcCZ.ke
        
          ExcCZ --> PU : ExcCZ.ke
          click PU href "../PU"
        
      ExcCZ : ExcCZ.kp
        
          ExcCZ --> PU : ExcCZ.kp
          click PU href "../PU"
        
      ExcCZ : IdentifiedObject.mRID
        
      ExcCZ : IdentifiedObject.name
        
      ExcCZ : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcCZ --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcCZ : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcCZ --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcCZ : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcCZ --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcCZ : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcCZ --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcCZ : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcCZ --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcCZ : ExcCZ.ta
        
          ExcCZ --> Seconds : ExcCZ.ta
          click Seconds href "../Seconds"
        
      ExcCZ : ExcCZ.tc
        
          ExcCZ --> Seconds : ExcCZ.tc
          click Seconds href "../Seconds"
        
      ExcCZ : ExcCZ.te
        
          ExcCZ --> Seconds : ExcCZ.te
          click Seconds href "../Seconds"
        
      ExcCZ : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcCZ --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcCZ : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcCZ --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcCZ : ExcCZ.vrmax
        
          ExcCZ --> PU : ExcCZ.vrmax
          click PU href "../PU"
        
      ExcCZ : ExcCZ.vrmin
        
          ExcCZ --> PU : ExcCZ.vrmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcCZ**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| kp | [cim:ExcCZ.kp](http://iec.ch/TC57/CIM100#ExcCZ.kp) | 1 <br />  [PU](PU.md)  | Regulator proportional gain (<i>Kp</i>) | direct |
| tc | [cim:ExcCZ.tc](http://iec.ch/TC57/CIM100#ExcCZ.tc) | 1 <br />  [Seconds](Seconds.md)  | Regulator integral time constant (<i>Tc</i>) (&gt;= 0) | direct |
| vrmax | [cim:ExcCZ.vrmax](http://iec.ch/TC57/CIM100#ExcCZ.vrmax) | 1 <br />  [PU](PU.md)  | Voltage regulator maximum limit (<i>Vrmax</i>) (&gt; ExcCZ | direct |
| vrmin | [cim:ExcCZ.vrmin](http://iec.ch/TC57/CIM100#ExcCZ.vrmin) | 1 <br />  [PU](PU.md)  | Voltage regulator minimum limit (<i>Vrmin</i>) (&lt; ExcCZ | direct |
| ka | [cim:ExcCZ.ka](http://iec.ch/TC57/CIM100#ExcCZ.ka) | 1 <br />  [PU](PU.md)  | Regulator gain (<i>Ka</i>) | direct |
| ta | [cim:ExcCZ.ta](http://iec.ch/TC57/CIM100#ExcCZ.ta) | 1 <br />  [Seconds](Seconds.md)  | Regulator time constant (<i>Ta</i>) (&gt;= 0) | direct |
| ke | [cim:ExcCZ.ke](http://iec.ch/TC57/CIM100#ExcCZ.ke) | 1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| te | [cim:ExcCZ.te](http://iec.ch/TC57/CIM100#ExcCZ.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| efdmax | [cim:ExcCZ.efdmax](http://iec.ch/TC57/CIM100#ExcCZ.efdmax) | 1 <br />  [PU](PU.md)  | Exciter output maximum limit (<i>Efdmax</i>) (&gt; ExcCZ | direct |
| efdmin | [cim:ExcCZ.efdmin](http://iec.ch/TC57/CIM100#ExcCZ.efdmin) | 1 <br />  [PU](PU.md)  | Exciter output minimum limit (<i>Efdmin</i>) (&lt; ExcCZ | direct |
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
| self | cim:ExcCZ |
| native | this:ExcCZ |




