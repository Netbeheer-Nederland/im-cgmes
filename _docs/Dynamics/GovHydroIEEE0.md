# GovHydroIEEE0


_IEEE simplified hydro governor-turbine model.  Used for mechanical-hydraulic and electro-hydraulic turbine governors, with or without steam feedback. Typical values given are for mechanical-hydraulic turbine-governor._

_Ref<font color="#0f0f0f">erence: IEEE Transactions on Power Apparatus and Systems, November/December 1973, Volume PAS-92, Number 6, <i><u>Dynamic Models for Steam and Hydro Turbines in Power System Studies</u></i>, page 1904.</font>_





**URI**: [cim:GovHydroIEEE0](http://iec.ch/TC57/CIM100#GovHydroIEEE0)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovHydroIEEE0
      TurbineGovernorDynamics <|-- GovHydroIEEE0
      
      GovHydroIEEE0 : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovHydroIEEE0 --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
      GovHydroIEEE0 : IdentifiedObject.description
        
      GovHydroIEEE0 : DynamicsFunctionBlock.enabled
        
      GovHydroIEEE0 : GovHydroIEEE0.k
        
          GovHydroIEEE0 --> PU : GovHydroIEEE0.k
        
      GovHydroIEEE0 : IdentifiedObject.mRID
        
      GovHydroIEEE0 : GovHydroIEEE0.mwbase
        
          GovHydroIEEE0 --> ActivePower : GovHydroIEEE0.mwbase
        
      GovHydroIEEE0 : IdentifiedObject.name
        
      GovHydroIEEE0 : GovHydroIEEE0.pmax
        
          GovHydroIEEE0 --> PU : GovHydroIEEE0.pmax
        
      GovHydroIEEE0 : GovHydroIEEE0.pmin
        
          GovHydroIEEE0 --> PU : GovHydroIEEE0.pmin
        
      GovHydroIEEE0 : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovHydroIEEE0 --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
        
      GovHydroIEEE0 : GovHydroIEEE0.t1
        
          GovHydroIEEE0 --> Seconds : GovHydroIEEE0.t1
        
      GovHydroIEEE0 : GovHydroIEEE0.t2
        
          GovHydroIEEE0 --> Seconds : GovHydroIEEE0.t2
        
      GovHydroIEEE0 : GovHydroIEEE0.t3
        
          GovHydroIEEE0 --> Seconds : GovHydroIEEE0.t3
        
      GovHydroIEEE0 : GovHydroIEEE0.t4
        
          GovHydroIEEE0 --> Seconds : GovHydroIEEE0.t4
        
      GovHydroIEEE0 : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovHydroIEEE0 --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovHydroIEEE0**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mwbase | [cim:GovHydroIEEE0.mwbase](http://iec.ch/TC57/CIM100#GovHydroIEEE0.mwbase) | 1..1 <br />  [ActivePower](ActivePower.md)  | Base for power values (<i>MWbase</i>) (&gt; 0) | direct |
| k | [cim:GovHydroIEEE0.k](http://iec.ch/TC57/CIM100#GovHydroIEEE0.k) | 1..1 <br />  [PU](PU.md)  | Governor gain (<i>K)</i> | direct |
| t1 | [cim:GovHydroIEEE0.t1](http://iec.ch/TC57/CIM100#GovHydroIEEE0.t1) | 1..1 <br />  [Seconds](Seconds.md)  | Governor lag time constant (<i>T1</i>) (&gt;= 0) | direct |
| t2 | [cim:GovHydroIEEE0.t2](http://iec.ch/TC57/CIM100#GovHydroIEEE0.t2) | 1..1 <br />  [Seconds](Seconds.md)  | Governor lead time constant (<i>T2)</i> (&gt;= 0) | direct |
| t3 | [cim:GovHydroIEEE0.t3](http://iec.ch/TC57/CIM100#GovHydroIEEE0.t3) | 1..1 <br />  [Seconds](Seconds.md)  | Gate actuator time constant (<i>T3</i>) (&gt;= 0) | direct |
| t4 | [cim:GovHydroIEEE0.t4](http://iec.ch/TC57/CIM100#GovHydroIEEE0.t4) | 1..1 <br />  [Seconds](Seconds.md)  | Water starting time (<i>T4</i>) (&gt;= 0) | direct |
| pmax | [cim:GovHydroIEEE0.pmax](http://iec.ch/TC57/CIM100#GovHydroIEEE0.pmax) | 1..1 <br />  [PU](PU.md)  | Gate maximum (<i>Pmax</i>) (&gt; GovHydroIEEE0 | direct |
| pmin | [cim:GovHydroIEEE0.pmin](http://iec.ch/TC57/CIM100#GovHydroIEEE0.pmin) | 1..1 <br />  [PU](PU.md)  | Gate minimum (<i>Pmin</i>) (&lt; GovHydroIEEE | direct |
| SynchronousMachineDynamics | [cim:TurbineGovernorDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.SynchronousMachineDynamics) | 0..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this turbine-governor model is associate... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| AsynchronousMachineDynamics | [cim:TurbineGovernorDynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.AsynchronousMachineDynamics) | 0..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this turbine-governor model is associat... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| TurbineLoadControllerDynamics | [cim:TurbineGovernorDynamics.TurbineLoadControllerDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.TurbineLoadControllerDynamics) | 0..1 <br />  [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md)  | Turbine load controller providing input to this turbine-governor | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
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
| self | cim:GovHydroIEEE0 |
| native | this:GovHydroIEEE0 |




