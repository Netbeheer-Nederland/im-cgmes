# ExcST4B


_Modified IEEE ST4B static excitation system with maximum inner loop feedback gain <i>Vgmax</i>._





**URI**: [cim:ExcST4B](http://iec.ch/TC57/CIM100#ExcST4B)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcST4B
    click ExcST4B href "../ExcST4B"
      ExcitationSystemDynamics <|-- ExcST4B
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcST4B : IdentifiedObject.description
        
      ExcST4B : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcST4B --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcST4B : DynamicsFunctionBlock.enabled
        
      ExcST4B : ExcST4B.kc
        
          ExcST4B --> PU : ExcST4B.kc
          click PU href "../PU"
        
      ExcST4B : ExcST4B.kg
        
          ExcST4B --> PU : ExcST4B.kg
          click PU href "../PU"
        
      ExcST4B : ExcST4B.ki
        
          ExcST4B --> PU : ExcST4B.ki
          click PU href "../PU"
        
      ExcST4B : ExcST4B.kim
        
          ExcST4B --> PU : ExcST4B.kim
          click PU href "../PU"
        
      ExcST4B : ExcST4B.kir
        
          ExcST4B --> PU : ExcST4B.kir
          click PU href "../PU"
        
      ExcST4B : ExcST4B.kp
        
          ExcST4B --> PU : ExcST4B.kp
          click PU href "../PU"
        
      ExcST4B : ExcST4B.kpm
        
          ExcST4B --> PU : ExcST4B.kpm
          click PU href "../PU"
        
      ExcST4B : ExcST4B.kpr
        
          ExcST4B --> PU : ExcST4B.kpr
          click PU href "../PU"
        
      ExcST4B : ExcST4B.lvgate
        
      ExcST4B : IdentifiedObject.mRID
        
      ExcST4B : IdentifiedObject.name
        
      ExcST4B : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcST4B --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcST4B : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcST4B --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcST4B : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcST4B --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcST4B : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcST4B --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcST4B : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcST4B --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcST4B : ExcST4B.ta
        
          ExcST4B --> Seconds : ExcST4B.ta
          click Seconds href "../Seconds"
        
      ExcST4B : ExcST4B.thetap
        
          ExcST4B --> AngleDegrees : ExcST4B.thetap
          click AngleDegrees href "../AngleDegrees"
        
      ExcST4B : ExcST4B.uel
        
      ExcST4B : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcST4B --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcST4B : ExcST4B.vbmax
        
          ExcST4B --> PU : ExcST4B.vbmax
          click PU href "../PU"
        
      ExcST4B : ExcST4B.vgmax
        
          ExcST4B --> PU : ExcST4B.vgmax
          click PU href "../PU"
        
      ExcST4B : ExcST4B.vmmax
        
          ExcST4B --> PU : ExcST4B.vmmax
          click PU href "../PU"
        
      ExcST4B : ExcST4B.vmmin
        
          ExcST4B --> PU : ExcST4B.vmmin
          click PU href "../PU"
        
      ExcST4B : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcST4B --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcST4B : ExcST4B.vrmax
        
          ExcST4B --> PU : ExcST4B.vrmax
          click PU href "../PU"
        
      ExcST4B : ExcST4B.vrmin
        
          ExcST4B --> PU : ExcST4B.vrmin
          click PU href "../PU"
        
      ExcST4B : ExcST4B.xl
        
          ExcST4B --> PU : ExcST4B.xl
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcST4B**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| kpr | [cim:ExcST4B.kpr](http://iec.ch/TC57/CIM100#ExcST4B.kpr) | 1 <br />  [PU](PU.md)  | Voltage regulator proportional gain (<i>Kpr</i>) | direct |
| kir | [cim:ExcST4B.kir](http://iec.ch/TC57/CIM100#ExcST4B.kir) | 1 <br />  [PU](PU.md)  | Voltage regulator integral gain (<i>Kir</i>) | direct |
| ta | [cim:ExcST4B.ta](http://iec.ch/TC57/CIM100#ExcST4B.ta) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt;= 0) | direct |
| vrmax | [cim:ExcST4B.vrmax](http://iec.ch/TC57/CIM100#ExcST4B.vrmax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vrmax</i>) (&gt; 0) | direct |
| vrmin | [cim:ExcST4B.vrmin](http://iec.ch/TC57/CIM100#ExcST4B.vrmin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vrmin</i>) (&lt; 0) | direct |
| kpm | [cim:ExcST4B.kpm](http://iec.ch/TC57/CIM100#ExcST4B.kpm) | 1 <br />  [PU](PU.md)  | Voltage regulator proportional gain output (<i>Kpm</i>) | direct |
| kim | [cim:ExcST4B.kim](http://iec.ch/TC57/CIM100#ExcST4B.kim) | 1 <br />  [PU](PU.md)  | Voltage regulator integral gain output (<i>Kim</i>) | direct |
| vmmax | [cim:ExcST4B.vmmax](http://iec.ch/TC57/CIM100#ExcST4B.vmmax) | 1 <br />  [PU](PU.md)  | Maximum inner loop output (<i>Vmmax</i>) (&gt; ExcST4B | direct |
| vmmin | [cim:ExcST4B.vmmin](http://iec.ch/TC57/CIM100#ExcST4B.vmmin) | 1 <br />  [PU](PU.md)  | Minimum inner loop output (<i>Vmmin</i>) (&lt; ExcST4B | direct |
| kg | [cim:ExcST4B.kg](http://iec.ch/TC57/CIM100#ExcST4B.kg) | 1 <br />  [PU](PU.md)  | Feedback gain constant of the inner loop field regulator (<i>Kg</i>) (&gt;= 0... | direct |
| kp | [cim:ExcST4B.kp](http://iec.ch/TC57/CIM100#ExcST4B.kp) | 1 <br />  [PU](PU.md)  | Potential circuit gain coefficient (<i>Kp</i>) (&gt; 0) | direct |
| thetap | [cim:ExcST4B.thetap](http://iec.ch/TC57/CIM100#ExcST4B.thetap) | 1 <br />  [AngleDegrees](AngleDegrees.md)  | Potential circuit phase angle (<i>theta</i><i><sub>p</sub></i>) | direct |
| ki | [cim:ExcST4B.ki](http://iec.ch/TC57/CIM100#ExcST4B.ki) | 1 <br />  [PU](PU.md)  | Potential circuit gain coefficient (<i>Ki</i>) (&gt;= 0) | direct |
| kc | [cim:ExcST4B.kc](http://iec.ch/TC57/CIM100#ExcST4B.kc) | 1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| xl | [cim:ExcST4B.xl](http://iec.ch/TC57/CIM100#ExcST4B.xl) | 1 <br />  [PU](PU.md)  | Reactance associated with potential source (<i>Xl</i>) (&gt;= 0) | direct |
| vbmax | [cim:ExcST4B.vbmax](http://iec.ch/TC57/CIM100#ExcST4B.vbmax) | 1 <br />  [PU](PU.md)  | Maximum excitation voltage (<i>Vbmax</i>) (&gt; 0) | direct |
| vgmax | [cim:ExcST4B.vgmax](http://iec.ch/TC57/CIM100#ExcST4B.vgmax) | 1 <br />  [PU](PU.md)  | Maximum inner loop feedback voltage (<i>Vgmax</i>) (&gt;= 0) | direct |
| uel | [cim:ExcST4B.uel](http://iec.ch/TC57/CIM100#ExcST4B.uel) | 1 <br />  boolean  | Selector (<i>UEL</i>) | direct |
| lvgate | [cim:ExcST4B.lvgate](http://iec.ch/TC57/CIM100#ExcST4B.lvgate) | 1 <br />  boolean  | Selector (<i>LVGate</i>) | direct |
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
| self | cim:ExcST4B |
| native | this:ExcST4B |




