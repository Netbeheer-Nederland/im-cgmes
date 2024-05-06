# GovSteamIEEE1


_IEEE steam turbine governor model._

_Ref<font color="#0f0f0f">erence: IEEE Transactions on Power Apparatus and Systems, November/December 1973, Volume PAS-92, Number 6, <i><u>Dynamic Models for Steam and Hydro Turbines in Power System Studies</u></i>, page 1904.</font>_





**URI**: [cim:GovSteamIEEE1](http://iec.ch/TC57/CIM100#GovSteamIEEE1)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovSteamIEEE1
    click GovSteamIEEE1 href "../GovSteamIEEE1"
      TurbineGovernorDynamics <|-- GovSteamIEEE1
        click TurbineGovernorDynamics href "../TurbineGovernorDynamics"
      
      GovSteamIEEE1 : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovSteamIEEE1 --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      GovSteamIEEE1 : IdentifiedObject.description
        
      GovSteamIEEE1 : DynamicsFunctionBlock.enabled
        
      GovSteamIEEE1 : GovSteamIEEE1.k
        
          GovSteamIEEE1 --> PU : GovSteamIEEE1.k
          click PU href "../PU"
        
      GovSteamIEEE1 : GovSteamIEEE1.k1
        
      GovSteamIEEE1 : GovSteamIEEE1.k2
        
      GovSteamIEEE1 : GovSteamIEEE1.k3
        
      GovSteamIEEE1 : GovSteamIEEE1.k4
        
      GovSteamIEEE1 : GovSteamIEEE1.k5
        
      GovSteamIEEE1 : GovSteamIEEE1.k6
        
      GovSteamIEEE1 : GovSteamIEEE1.k7
        
      GovSteamIEEE1 : GovSteamIEEE1.k8
        
      GovSteamIEEE1 : IdentifiedObject.mRID
        
      GovSteamIEEE1 : GovSteamIEEE1.mwbase
        
          GovSteamIEEE1 --> ActivePower : GovSteamIEEE1.mwbase
          click ActivePower href "../ActivePower"
        
      GovSteamIEEE1 : IdentifiedObject.name
        
      GovSteamIEEE1 : GovSteamIEEE1.pmax
        
          GovSteamIEEE1 --> PU : GovSteamIEEE1.pmax
          click PU href "../PU"
        
      GovSteamIEEE1 : GovSteamIEEE1.pmin
        
          GovSteamIEEE1 --> PU : GovSteamIEEE1.pmin
          click PU href "../PU"
        
      GovSteamIEEE1 : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovSteamIEEE1 --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      GovSteamIEEE1 : GovSteamIEEE1.t1
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t1
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : GovSteamIEEE1.t2
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t2
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : GovSteamIEEE1.t3
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t3
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : GovSteamIEEE1.t4
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t4
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : GovSteamIEEE1.t5
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t5
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : GovSteamIEEE1.t6
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t6
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : GovSteamIEEE1.t7
        
          GovSteamIEEE1 --> Seconds : GovSteamIEEE1.t7
          click Seconds href "../Seconds"
        
      GovSteamIEEE1 : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovSteamIEEE1 --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
          click TurbineLoadControllerDynamics href "../TurbineLoadControllerDynamics"
        
      GovSteamIEEE1 : GovSteamIEEE1.uc
        
      GovSteamIEEE1 : GovSteamIEEE1.uo
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovSteamIEEE1**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mwbase | [cim:GovSteamIEEE1.mwbase](http://iec.ch/TC57/CIM100#GovSteamIEEE1.mwbase) | 1 <br />  [ActivePower](ActivePower.md)  | Base for power values (<i>MWbase</i>) (&gt; 0)<i> | direct |
| k | [cim:GovSteamIEEE1.k](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k) | 1 <br />  [PU](PU.md)  | Governor gain (reciprocal of droop) (<i>K</i>) (&gt; 0) | direct |
| t1 | [cim:GovSteamIEEE1.t1](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t1) | 1 <br />  [Seconds](Seconds.md)  | Governor lag time constant (<i>T1</i>) (&gt;= 0) | direct |
| t2 | [cim:GovSteamIEEE1.t2](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t2) | 1 <br />  [Seconds](Seconds.md)  | Governor lead time constant (<i>T2</i>) (&gt;= 0) | direct |
| t3 | [cim:GovSteamIEEE1.t3](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t3) | 1 <br />  [Seconds](Seconds.md)  | Valve positioner time constant (<i>T3</i>) (&gt; 0) | direct |
| uo | [cim:GovSteamIEEE1.uo](http://iec.ch/TC57/CIM100#GovSteamIEEE1.uo) | 1 <br />  float  | Maximum valve opening velocity (<i>Uo</i>) (&gt; 0) | direct |
| uc | [cim:GovSteamIEEE1.uc](http://iec.ch/TC57/CIM100#GovSteamIEEE1.uc) | 1 <br />  float  | Maximum valve closing velocity (<i>Uc</i>) (&lt; 0) | direct |
| pmax | [cim:GovSteamIEEE1.pmax](http://iec.ch/TC57/CIM100#GovSteamIEEE1.pmax) | 1 <br />  [PU](PU.md)  | Maximum valve opening (<i>Pmax</i>) (&gt; GovSteamIEEE1 | direct |
| pmin | [cim:GovSteamIEEE1.pmin](http://iec.ch/TC57/CIM100#GovSteamIEEE1.pmin) | 1 <br />  [PU](PU.md)  | Minimum valve opening (<i>Pmin</i>) (&gt;= 0 and &lt; GovSteamIEEE1 | direct |
| t4 | [cim:GovSteamIEEE1.t4](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t4) | 1 <br />  [Seconds](Seconds.md)  | Inlet piping/steam bowl time constant (<i>T4</i>) (&gt;= 0) | direct |
| k1 | [cim:GovSteamIEEE1.k1](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k1) | 1 <br />  float  | Fraction of HP shaft power after first boiler pass (<i>K1</i>) | direct |
| k2 | [cim:GovSteamIEEE1.k2](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k2) | 1 <br />  float  | Fraction of LP shaft power after first boiler pass (<i>K2</i>) | direct |
| t5 | [cim:GovSteamIEEE1.t5](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t5) | 1 <br />  [Seconds](Seconds.md)  | Time constant of second boiler pass (<i>T5</i>) (&gt;= 0) | direct |
| k3 | [cim:GovSteamIEEE1.k3](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k3) | 1 <br />  float  | Fraction of HP shaft power after second boiler pass (<i>K3</i>) | direct |
| k4 | [cim:GovSteamIEEE1.k4](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k4) | 1 <br />  float  | Fraction of LP shaft power after second boiler pass (<i>K4</i>) | direct |
| t6 | [cim:GovSteamIEEE1.t6](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t6) | 1 <br />  [Seconds](Seconds.md)  | Time constant of third boiler pass (<i>T6</i>) (&gt;= 0) | direct |
| k5 | [cim:GovSteamIEEE1.k5](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k5) | 1 <br />  float  | Fraction of HP shaft power after third boiler pass (<i>K5</i>) | direct |
| k6 | [cim:GovSteamIEEE1.k6](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k6) | 1 <br />  float  | Fraction of LP shaft power after third boiler pass (<i>K6</i>) | direct |
| t7 | [cim:GovSteamIEEE1.t7](http://iec.ch/TC57/CIM100#GovSteamIEEE1.t7) | 1 <br />  [Seconds](Seconds.md)  | Time constant of fourth boiler pass (<i>T7</i>) (&gt;= 0) | direct |
| k7 | [cim:GovSteamIEEE1.k7](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k7) | 1 <br />  float  | Fraction of HP shaft power after fourth boiler pass (<i>K7</i>) | direct |
| k8 | [cim:GovSteamIEEE1.k8](http://iec.ch/TC57/CIM100#GovSteamIEEE1.k8) | 1 <br />  float  | Fraction of LP shaft power after fourth boiler pass (<i>K8</i>) | direct |
| SynchronousMachineDynamics | [cim:TurbineGovernorDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.SynchronousMachineDynamics) | 0..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this turbine-governor model is associate... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| AsynchronousMachineDynamics | [cim:TurbineGovernorDynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.AsynchronousMachineDynamics) | 0..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this turbine-governor model is associat... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| TurbineLoadControllerDynamics | [cim:TurbineGovernorDynamics.TurbineLoadControllerDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.TurbineLoadControllerDynamics) | 0..1 <br />  [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md)  | Turbine load controller providing input to this turbine-governor | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
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
| self | cim:GovSteamIEEE1 |
| native | this:GovSteamIEEE1 |




