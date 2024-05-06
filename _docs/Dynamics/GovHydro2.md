# GovHydro2


_IEEE hydro turbine governor with straightforward penstock configuration and hydraulic-dashpot governor._





**URI**: [cim:GovHydro2](http://iec.ch/TC57/CIM100#GovHydro2)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovHydro2
    click GovHydro2 href "../GovHydro2"
      TurbineGovernorDynamics <|-- GovHydro2
        click TurbineGovernorDynamics href "../TurbineGovernorDynamics"
      
      GovHydro2 : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovHydro2 --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      GovHydro2 : GovHydro2.aturb
        
          GovHydro2 --> PU : GovHydro2.aturb
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.bturb
        
          GovHydro2 --> PU : GovHydro2.bturb
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.db1
        
          GovHydro2 --> Frequency : GovHydro2.db1
          click Frequency href "../Frequency"
        
      GovHydro2 : GovHydro2.db2
        
          GovHydro2 --> ActivePower : GovHydro2.db2
          click ActivePower href "../ActivePower"
        
      GovHydro2 : IdentifiedObject.description
        
      GovHydro2 : DynamicsFunctionBlock.enabled
        
      GovHydro2 : GovHydro2.eps
        
          GovHydro2 --> Frequency : GovHydro2.eps
          click Frequency href "../Frequency"
        
      GovHydro2 : GovHydro2.gv1
        
          GovHydro2 --> PU : GovHydro2.gv1
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.gv2
        
          GovHydro2 --> PU : GovHydro2.gv2
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.gv3
        
          GovHydro2 --> PU : GovHydro2.gv3
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.gv4
        
          GovHydro2 --> PU : GovHydro2.gv4
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.gv5
        
          GovHydro2 --> PU : GovHydro2.gv5
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.gv6
        
          GovHydro2 --> PU : GovHydro2.gv6
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.kturb
        
          GovHydro2 --> PU : GovHydro2.kturb
          click PU href "../PU"
        
      GovHydro2 : IdentifiedObject.mRID
        
      GovHydro2 : GovHydro2.mwbase
        
          GovHydro2 --> ActivePower : GovHydro2.mwbase
          click ActivePower href "../ActivePower"
        
      GovHydro2 : IdentifiedObject.name
        
      GovHydro2 : GovHydro2.pgv1
        
          GovHydro2 --> PU : GovHydro2.pgv1
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pgv2
        
          GovHydro2 --> PU : GovHydro2.pgv2
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pgv3
        
          GovHydro2 --> PU : GovHydro2.pgv3
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pgv4
        
          GovHydro2 --> PU : GovHydro2.pgv4
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pgv5
        
          GovHydro2 --> PU : GovHydro2.pgv5
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pgv6
        
          GovHydro2 --> PU : GovHydro2.pgv6
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pmax
        
          GovHydro2 --> PU : GovHydro2.pmax
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.pmin
        
          GovHydro2 --> PU : GovHydro2.pmin
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.rperm
        
          GovHydro2 --> PU : GovHydro2.rperm
          click PU href "../PU"
        
      GovHydro2 : GovHydro2.rtemp
        
          GovHydro2 --> PU : GovHydro2.rtemp
          click PU href "../PU"
        
      GovHydro2 : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovHydro2 --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      GovHydro2 : GovHydro2.tg
        
          GovHydro2 --> Seconds : GovHydro2.tg
          click Seconds href "../Seconds"
        
      GovHydro2 : GovHydro2.tp
        
          GovHydro2 --> Seconds : GovHydro2.tp
          click Seconds href "../Seconds"
        
      GovHydro2 : GovHydro2.tr
        
          GovHydro2 --> Seconds : GovHydro2.tr
          click Seconds href "../Seconds"
        
      GovHydro2 : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovHydro2 --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
          click TurbineLoadControllerDynamics href "../TurbineLoadControllerDynamics"
        
      GovHydro2 : GovHydro2.tw
        
          GovHydro2 --> Seconds : GovHydro2.tw
          click Seconds href "../Seconds"
        
      GovHydro2 : GovHydro2.uc
        
      GovHydro2 : GovHydro2.uo
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovHydro2**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mwbase | [cim:GovHydro2.mwbase](http://iec.ch/TC57/CIM100#GovHydro2.mwbase) | 1 <br />  [ActivePower](ActivePower.md)  | Base for power values (<i>MWbase</i>) (&gt; 0) | direct |
| tg | [cim:GovHydro2.tg](http://iec.ch/TC57/CIM100#GovHydro2.tg) | 1 <br />  [Seconds](Seconds.md)  | Gate servo time constant (<i>Tg</i>) (&gt; 0) | direct |
| tp | [cim:GovHydro2.tp](http://iec.ch/TC57/CIM100#GovHydro2.tp) | 1 <br />  [Seconds](Seconds.md)  | Pilot servo valve time constant (<i>Tp</i>) (&gt;= 0) | direct |
| uo | [cim:GovHydro2.uo](http://iec.ch/TC57/CIM100#GovHydro2.uo) | 1 <br />  float  | Maximum gate opening velocity (<i>Uo</i>) | direct |
| uc | [cim:GovHydro2.uc](http://iec.ch/TC57/CIM100#GovHydro2.uc) | 1 <br />  float  | Maximum gate closing velocity (<i>Uc</i>) (&lt; 0) | direct |
| pmax | [cim:GovHydro2.pmax](http://iec.ch/TC57/CIM100#GovHydro2.pmax) | 1 <br />  [PU](PU.md)  | Maximum gate opening (<i>Pmax</i>) (&gt; GovHydro2 | direct |
| pmin | [cim:GovHydro2.pmin](http://iec.ch/TC57/CIM100#GovHydro2.pmin) | 1 <br />  [PU](PU.md)  | Minimum gate opening (<i>Pmin</i>) (&lt; GovHydro2 | direct |
| rperm | [cim:GovHydro2.rperm](http://iec.ch/TC57/CIM100#GovHydro2.rperm) | 1 <br />  [PU](PU.md)  | Permanent droop (<i>Rperm</i>) | direct |
| rtemp | [cim:GovHydro2.rtemp](http://iec.ch/TC57/CIM100#GovHydro2.rtemp) | 1 <br />  [PU](PU.md)  | Temporary droop (<i>Rtemp</i>) | direct |
| tr | [cim:GovHydro2.tr](http://iec.ch/TC57/CIM100#GovHydro2.tr) | 1 <br />  [Seconds](Seconds.md)  | Dashpot time constant (<i>Tr</i>) (&gt;= 0) | direct |
| tw | [cim:GovHydro2.tw](http://iec.ch/TC57/CIM100#GovHydro2.tw) | 1 <br />  [Seconds](Seconds.md)  | Water inertia time constant (<i>Tw</i>) (&gt;= 0) | direct |
| kturb | [cim:GovHydro2.kturb](http://iec.ch/TC57/CIM100#GovHydro2.kturb) | 1 <br />  [PU](PU.md)  | Turbine gain (<i>Kturb</i>) | direct |
| aturb | [cim:GovHydro2.aturb](http://iec.ch/TC57/CIM100#GovHydro2.aturb) | 1 <br />  [PU](PU.md)  | Turbine numerator multiplier (<i>Aturb</i>) | direct |
| bturb | [cim:GovHydro2.bturb](http://iec.ch/TC57/CIM100#GovHydro2.bturb) | 1 <br />  [PU](PU.md)  | Turbine denominator multiplier (<i>Bturb</i>) (&gt; 0) | direct |
| db1 | [cim:GovHydro2.db1](http://iec.ch/TC57/CIM100#GovHydro2.db1) | 1 <br />  [Frequency](Frequency.md)  | Intentional deadband width (<i>db1</i>) | direct |
| eps | [cim:GovHydro2.eps](http://iec.ch/TC57/CIM100#GovHydro2.eps) | 1 <br />  [Frequency](Frequency.md)  | Intentional db hysteresis (<i>eps</i>) | direct |
| db2 | [cim:GovHydro2.db2](http://iec.ch/TC57/CIM100#GovHydro2.db2) | 1 <br />  [ActivePower](ActivePower.md)  | Unintentional deadband (<i>db2</i>) | direct |
| gv1 | [cim:GovHydro2.gv1](http://iec.ch/TC57/CIM100#GovHydro2.gv1) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 1, PU gv (<i>Gv1</i>) | direct |
| pgv1 | [cim:GovHydro2.pgv1](http://iec.ch/TC57/CIM100#GovHydro2.pgv1) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 1, PU power (<i>Pgv1</i>) | direct |
| gv2 | [cim:GovHydro2.gv2](http://iec.ch/TC57/CIM100#GovHydro2.gv2) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 2, PU gv (<i>Gv2</i>) | direct |
| pgv2 | [cim:GovHydro2.pgv2](http://iec.ch/TC57/CIM100#GovHydro2.pgv2) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 2, PU power (<i>Pgv2</i>) | direct |
| gv3 | [cim:GovHydro2.gv3](http://iec.ch/TC57/CIM100#GovHydro2.gv3) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 3, PU gv (<i>Gv3</i>) | direct |
| pgv3 | [cim:GovHydro2.pgv3](http://iec.ch/TC57/CIM100#GovHydro2.pgv3) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 3, PU power (<i>Pgv3</i>) | direct |
| gv4 | [cim:GovHydro2.gv4](http://iec.ch/TC57/CIM100#GovHydro2.gv4) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 4, PU gv (<i>Gv4</i>) | direct |
| pgv4 | [cim:GovHydro2.pgv4](http://iec.ch/TC57/CIM100#GovHydro2.pgv4) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 4, PU power (P<i>gv4</i>) | direct |
| gv5 | [cim:GovHydro2.gv5](http://iec.ch/TC57/CIM100#GovHydro2.gv5) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 5, PU gv (<i>Gv5</i>) | direct |
| pgv5 | [cim:GovHydro2.pgv5](http://iec.ch/TC57/CIM100#GovHydro2.pgv5) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 5, PU power (<i>Pgv5</i>) | direct |
| gv6 | [cim:GovHydro2.gv6](http://iec.ch/TC57/CIM100#GovHydro2.gv6) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 6, PU gv (<i>Gv6</i>) | direct |
| pgv6 | [cim:GovHydro2.pgv6](http://iec.ch/TC57/CIM100#GovHydro2.pgv6) | 1 <br />  [PU](PU.md)  | Nonlinear gain point 6, PU power (<i>Pgv6</i>) | direct |
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
| self | cim:GovHydro2 |
| native | this:GovHydro2 |




