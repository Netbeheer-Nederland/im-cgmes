# AsynchronousMachineEquivalentCircuit


_The electrical equations of all variations of the asynchronous model are based on the AsynchronousEquivalentCircuit diagram for the direct- and quadrature- axes, with two equivalent rotor windings in each axis.  _

_Equations for conversion between equivalent circuit and time constant reactance forms:_

_<i>Xs</i> = <i>Xm</i> + <i>Xl</i>_

_<i>X'</i> = <i>Xl</i> + <i>Xm</i> x <i>Xlr1 </i>/ (<i>Xm </i>+ <i>Xlr1</i>)_

_<i>X''</i> = <i>Xl</i> + <i>Xm</i> x <i>Xlr1</i> x <i>Xlr2</i> / (<i>Xm</i> x <i>Xlr1</i> + <i>Xm</i> x <i>Xlr2</i> + <i>Xlr1</i> x <i>Xlr2</i>)_

_<i>T'o</i> = (<i>Xm</i> + <i>Xlr1</i>) / (<i>omega</i><i><sub>0</sub></i> x <i>Rr1</i>)_

_<i>T''o</i> = (<i>Xm</i> x <i>Xlr1</i> + <i>Xm</i> x <i>Xlr2</i> + <i>Xlr1</i> x <i>Xlr2</i>) / (<i>omega</i><i><sub>0</sub></i> x <i>Rr2</i> x (<i>Xm</i> + <i>Xlr1</i>)_

_Same equations using CIM attributes from AsynchronousMachineTimeConstantReactance class on left of "=" and AsynchronousMachineEquivalentCircuit class on right (except as noted):_

_xs = xm + RotatingMachineDynamics.statorLeakageReactance_

_xp = RotatingMachineDynamics.statorLeakageReactance + xm x xlr1 / (xm + xlr1)_

_xpp = RotatingMachineDynamics.statorLeakageReactance + xm x xlr1 x xlr2 / (xm x xlr1 + xm x xlr2 + xlr1 x xlr2)_

_tpo = (xm + xlr1) / (2 x pi x nominal frequency x rr1)_

_tppo = (xm x xlr1 + xm x xlr2 + xlr1 x xlr2) / (2 x pi x nominal frequency x rr2 x (xm + xlr1)._





**URI**: [cim:AsynchronousMachineEquivalentCircuit](http://iec.ch/TC57/CIM100#AsynchronousMachineEquivalentCircuit)<br />
**Type**: Class




```mermaid
 classDiagram
    class AsynchronousMachineEquivalentCircuit
    click AsynchronousMachineEquivalentCircuit href "../AsynchronousMachineEquivalentCircuit"
      AsynchronousMachineDynamics <|-- AsynchronousMachineEquivalentCircuit
        click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
      
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineDynamics.AsynchronousMachine
        
          AsynchronousMachineEquivalentCircuit --> AsynchronousMachine : AsynchronousMachineDynamics.AsynchronousMachine
          click AsynchronousMachine href "../AsynchronousMachine"
        
      AsynchronousMachineEquivalentCircuit : RotatingMachineDynamics.damping
        
      AsynchronousMachineEquivalentCircuit : IdentifiedObject.description
        
      AsynchronousMachineEquivalentCircuit : DynamicsFunctionBlock.enabled
        
      AsynchronousMachineEquivalentCircuit : RotatingMachineDynamics.inertia
        
          AsynchronousMachineEquivalentCircuit --> Seconds : RotatingMachineDynamics.inertia
          click Seconds href "../Seconds"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineDynamics.MechanicalLoadDynamics
        
          AsynchronousMachineEquivalentCircuit --> MechanicalLoadDynamics : AsynchronousMachineDynamics.MechanicalLoadDynamics
          click MechanicalLoadDynamics href "../MechanicalLoadDynamics"
        
      AsynchronousMachineEquivalentCircuit : IdentifiedObject.mRID
        
      AsynchronousMachineEquivalentCircuit : IdentifiedObject.name
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineEquivalentCircuit.rr1
        
          AsynchronousMachineEquivalentCircuit --> PU : AsynchronousMachineEquivalentCircuit.rr1
          click PU href "../PU"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineEquivalentCircuit.rr2
        
          AsynchronousMachineEquivalentCircuit --> PU : AsynchronousMachineEquivalentCircuit.rr2
          click PU href "../PU"
        
      AsynchronousMachineEquivalentCircuit : RotatingMachineDynamics.saturationFactor
        
      AsynchronousMachineEquivalentCircuit : RotatingMachineDynamics.saturationFactor120
        
      AsynchronousMachineEquivalentCircuit : RotatingMachineDynamics.statorLeakageReactance
        
          AsynchronousMachineEquivalentCircuit --> PU : RotatingMachineDynamics.statorLeakageReactance
          click PU href "../PU"
        
      AsynchronousMachineEquivalentCircuit : RotatingMachineDynamics.statorResistance
        
          AsynchronousMachineEquivalentCircuit --> PU : RotatingMachineDynamics.statorResistance
          click PU href "../PU"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineDynamics.TurbineGovernorDynamics
        
          AsynchronousMachineEquivalentCircuit --> TurbineGovernorDynamics : AsynchronousMachineDynamics.TurbineGovernorDynamics
          click TurbineGovernorDynamics href "../TurbineGovernorDynamics"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineDynamics.WindTurbineType1or2Dynamics
        
          AsynchronousMachineEquivalentCircuit --> WindTurbineType1or2Dynamics : AsynchronousMachineDynamics.WindTurbineType1or2Dynamics
          click WindTurbineType1or2Dynamics href "../WindTurbineType1or2Dynamics"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineEquivalentCircuit.xlr1
        
          AsynchronousMachineEquivalentCircuit --> PU : AsynchronousMachineEquivalentCircuit.xlr1
          click PU href "../PU"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineEquivalentCircuit.xlr2
        
          AsynchronousMachineEquivalentCircuit --> PU : AsynchronousMachineEquivalentCircuit.xlr2
          click PU href "../PU"
        
      AsynchronousMachineEquivalentCircuit : AsynchronousMachineEquivalentCircuit.xm
        
          AsynchronousMachineEquivalentCircuit --> PU : AsynchronousMachineEquivalentCircuit.xm
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [RotatingMachineDynamics](RotatingMachineDynamics.md)
            * [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)
                * **AsynchronousMachineEquivalentCircuit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| xm | [cim:AsynchronousMachineEquivalentCircuit.xm](http://iec.ch/TC57/CIM100#AsynchronousMachineEquivalentCircuit.xm) | 1 <br />  [PU](PU.md)  | Magnetizing reactance | direct |
| rr1 | [cim:AsynchronousMachineEquivalentCircuit.rr1](http://iec.ch/TC57/CIM100#AsynchronousMachineEquivalentCircuit.rr1) | 1 <br />  [PU](PU.md)  | Damper 1 winding resistance | direct |
| xlr1 | [cim:AsynchronousMachineEquivalentCircuit.xlr1](http://iec.ch/TC57/CIM100#AsynchronousMachineEquivalentCircuit.xlr1) | 1 <br />  [PU](PU.md)  | Damper 1 winding leakage reactance | direct |
| rr2 | [cim:AsynchronousMachineEquivalentCircuit.rr2](http://iec.ch/TC57/CIM100#AsynchronousMachineEquivalentCircuit.rr2) | 1 <br />  [PU](PU.md)  | Damper 2 winding resistance | direct |
| xlr2 | [cim:AsynchronousMachineEquivalentCircuit.xlr2](http://iec.ch/TC57/CIM100#AsynchronousMachineEquivalentCircuit.xlr2) | 1 <br />  [PU](PU.md)  | Damper 2 winding leakage reactance | direct |
| AsynchronousMachine | [cim:AsynchronousMachineDynamics.AsynchronousMachine](http://iec.ch/TC57/CIM100#AsynchronousMachineDynamics.AsynchronousMachine) | 1 <br />  [AsynchronousMachine](AsynchronousMachine.md)  | Asynchronous machine to which this asynchronous machine dynamics model applie... | [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md) |
| TurbineGovernorDynamics | [cim:AsynchronousMachineDynamics.TurbineGovernorDynamics](http://iec.ch/TC57/CIM100#AsynchronousMachineDynamics.TurbineGovernorDynamics) | 0..1 <br />  [TurbineGovernorDynamics](TurbineGovernorDynamics.md)  | Turbine-governor model associated with this asynchronous machine model | [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md) |
| MechanicalLoadDynamics | [cim:AsynchronousMachineDynamics.MechanicalLoadDynamics](http://iec.ch/TC57/CIM100#AsynchronousMachineDynamics.MechanicalLoadDynamics) | 0..1 <br />  [MechanicalLoadDynamics](MechanicalLoadDynamics.md)  | Mechanical load model associated with this asynchronous machine model | [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md) |
| WindTurbineType1or2Dynamics | [cim:AsynchronousMachineDynamics.WindTurbineType1or2Dynamics](http://iec.ch/TC57/CIM100#AsynchronousMachineDynamics.WindTurbineType1or2Dynamics) | 0..1 <br />  [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md)  | Wind generator type 1 or type 2 model associated with this asynchronous machi... | [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md) |
| damping | [cim:RotatingMachineDynamics.damping](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.damping) | 1 <br />  float  | Damping torque coefficient (<i>D</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| inertia | [cim:RotatingMachineDynamics.inertia](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.inertia) | 1 <br />  [Seconds](Seconds.md)  | Inertia constant of generator or motor and mechanical load (<i>H</i>) (&gt; 0... | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| saturationFactor | [cim:RotatingMachineDynamics.saturationFactor](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.saturationFactor) | 0..1 <br />  float  | Saturation factor at rated terminal voltage (<i>S1</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| saturationFactor120 | [cim:RotatingMachineDynamics.saturationFactor120](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.saturationFactor120) | 0..1 <br />  float  | Saturation factor at 120% of rated terminal voltage (<i>S12</i>) (&gt;= Rotat... | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| statorLeakageReactance | [cim:RotatingMachineDynamics.statorLeakageReactance](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.statorLeakageReactance) | 1 <br />  [PU](PU.md)  | Stator leakage reactance (<i>Xl</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| statorResistance | [cim:RotatingMachineDynamics.statorResistance](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.statorResistance) | 1 <br />  [PU](PU.md)  | Stator (armature) resistance (<i>Rs</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
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
| self | cim:AsynchronousMachineEquivalentCircuit |
| native | this:AsynchronousMachineEquivalentCircuit |




