# PssSK


_Slovakian PSS with three inputs._





**URI**: [cim:PssSK](http://iec.ch/TC57/CIM100#PssSK)<br />
**Type**: Class




```mermaid
 classDiagram
    class PssSK
      PowerSystemStabilizerDynamics <|-- PssSK
      
      PssSK : IdentifiedObject.description
        
      PssSK : DynamicsFunctionBlock.enabled
        
      PssSK : PowerSystemStabilizerDynamics.ExcitationSystemDynamics
        
          PssSK --> ExcitationSystemDynamics : PowerSystemStabilizerDynamics.ExcitationSystemDynamics
        
      PssSK : PssSK.k1
        
          PssSK --> PU : PssSK.k1
        
      PssSK : PssSK.k2
        
          PssSK --> PU : PssSK.k2
        
      PssSK : PssSK.k3
        
          PssSK --> PU : PssSK.k3
        
      PssSK : IdentifiedObject.mRID
        
      PssSK : IdentifiedObject.name
        
      PssSK : PowerSystemStabilizerDynamics.RemoteInputSignal
        
          PssSK --> RemoteInputSignal : PowerSystemStabilizerDynamics.RemoteInputSignal
        
      PssSK : PssSK.t1
        
          PssSK --> Seconds : PssSK.t1
        
      PssSK : PssSK.t2
        
          PssSK --> Seconds : PssSK.t2
        
      PssSK : PssSK.t3
        
          PssSK --> Seconds : PssSK.t3
        
      PssSK : PssSK.t4
        
          PssSK --> Seconds : PssSK.t4
        
      PssSK : PssSK.t5
        
          PssSK --> Seconds : PssSK.t5
        
      PssSK : PssSK.t6
        
          PssSK --> Seconds : PssSK.t6
        
      PssSK : PssSK.vsmax
        
          PssSK --> PU : PssSK.vsmax
        
      PssSK : PssSK.vsmin
        
          PssSK --> PU : PssSK.vsmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)
            * **PssSK**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| k1 | [cim:PssSK.k1](http://iec.ch/TC57/CIM100#PssSK.k1) | 1..1 <br />  [PU](PU.md)  | Gain <i>P</i> (<i>K</i><i><sub>1</sub></i>) | direct |
| k2 | [cim:PssSK.k2](http://iec.ch/TC57/CIM100#PssSK.k2) | 1..1 <br />  [PU](PU.md)  | Gain <i>f</i><i><sub>E</sub></i><i> </i>(<i>K</i><i><sub>2</sub></i>) | direct |
| k3 | [cim:PssSK.k3](http://iec.ch/TC57/CIM100#PssSK.k3) | 1..1 <br />  [PU](PU.md)  | Gain <i>I</i><i><sub>f</sub></i><i> </i>(<i>K</i><i><sub>3</sub></i>) | direct |
| t1 | [cim:PssSK.t1](http://iec.ch/TC57/CIM100#PssSK.t1) | 1..1 <br />  [Seconds](Seconds.md)  | Denominator time constant (<i>T</i><i><sub>1</sub></i>) (&gt; 0,005) | direct |
| t2 | [cim:PssSK.t2](http://iec.ch/TC57/CIM100#PssSK.t2) | 1..1 <br />  [Seconds](Seconds.md)  | Filter time constant (<i>T</i><i><sub>2</sub></i>) (&gt; 0,005) | direct |
| t3 | [cim:PssSK.t3](http://iec.ch/TC57/CIM100#PssSK.t3) | 1..1 <br />  [Seconds](Seconds.md)  | Denominator time constant (<i>T</i><i><sub>3</sub></i>) (&gt; 0,005) | direct |
| t4 | [cim:PssSK.t4](http://iec.ch/TC57/CIM100#PssSK.t4) | 1..1 <br />  [Seconds](Seconds.md)  | Filter time constant (<i>T</i><i><sub>4</sub></i>) (&gt; 0,005) | direct |
| t5 | [cim:PssSK.t5](http://iec.ch/TC57/CIM100#PssSK.t5) | 1..1 <br />  [Seconds](Seconds.md)  | Denominator time constant (<i>T</i><i><sub>5</sub></i>) (&gt; 0,005) | direct |
| t6 | [cim:PssSK.t6](http://iec.ch/TC57/CIM100#PssSK.t6) | 1..1 <br />  [Seconds](Seconds.md)  | Filter time constant (<i>T</i><i><sub>6</sub></i>) (&gt; 0,005) | direct |
| vsmax | [cim:PssSK.vsmax](http://iec.ch/TC57/CIM100#PssSK.vsmax) | 1..1 <br />  [PU](PU.md)  | Stabilizer output maximum limit (<i>V</i><i><sub>SMAX</sub></i>) (&gt; PssSK | direct |
| vsmin | [cim:PssSK.vsmin](http://iec.ch/TC57/CIM100#PssSK.vsmin) | 1..1 <br />  [PU](PU.md)  | Stabilizer output minimum limit (<i>V</i><i><sub>SMIN</sub></i>) (&lt; PssSK | direct |
| RemoteInputSignal | [cim:PowerSystemStabilizerDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#PowerSystemStabilizerDynamics.RemoteInputSignal) | 0..* <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this power system stabilizer model | [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md) |
| ExcitationSystemDynamics | [cim:PowerSystemStabilizerDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PowerSystemStabilizerDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power system stabilizer model is asso... | [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md) |
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
| self | cim:PssSK |
| native | this:PssSK |




