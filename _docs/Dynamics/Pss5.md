# Pss5


_Detailed Italian PSS._





**URI**: [cim:Pss5](http://iec.ch/TC57/CIM100#Pss5)<br />
**Type**: Class




```mermaid
 classDiagram
    class Pss5
    click Pss5 href "../Pss5"
      PowerSystemStabilizerDynamics <|-- Pss5
        click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
      
      Pss5 : Pss5.ctw2
        
      Pss5 : Pss5.deadband
        
          Pss5 --> PU : Pss5.deadband
          click PU href "../PU"
        
      Pss5 : IdentifiedObject.description
        
      Pss5 : DynamicsFunctionBlock.enabled
        
      Pss5 : PowerSystemStabilizerDynamics.ExcitationSystemDynamics
        
          Pss5 --> ExcitationSystemDynamics : PowerSystemStabilizerDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      Pss5 : Pss5.isfreq
        
      Pss5 : Pss5.kf
        
      Pss5 : Pss5.kpe
        
      Pss5 : Pss5.kpss
        
      Pss5 : IdentifiedObject.mRID
        
      Pss5 : IdentifiedObject.name
        
      Pss5 : Pss5.pmin
        
          Pss5 --> PU : Pss5.pmin
          click PU href "../PU"
        
      Pss5 : PowerSystemStabilizerDynamics.RemoteInputSignal
        
          Pss5 --> RemoteInputSignal : PowerSystemStabilizerDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      Pss5 : Pss5.tl1
        
          Pss5 --> Seconds : Pss5.tl1
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.tl2
        
          Pss5 --> Seconds : Pss5.tl2
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.tl3
        
          Pss5 --> Seconds : Pss5.tl3
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.tl4
        
          Pss5 --> Seconds : Pss5.tl4
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.tpe
        
          Pss5 --> Seconds : Pss5.tpe
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.tw1
        
          Pss5 --> Seconds : Pss5.tw1
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.tw2
        
          Pss5 --> Seconds : Pss5.tw2
          click Seconds href "../Seconds"
        
      Pss5 : Pss5.vadat
        
      Pss5 : Pss5.vsmn
        
          Pss5 --> PU : Pss5.vsmn
          click PU href "../PU"
        
      Pss5 : Pss5.vsmx
        
          Pss5 --> PU : Pss5.vsmx
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)
            * **Pss5**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| kpe | [cim:Pss5.kpe](http://iec.ch/TC57/CIM100#Pss5.kpe) | 1 <br />  float  | Electric power input gain (<i>K</i><i><sub>PE</sub></i>) | direct |
| kf | [cim:Pss5.kf](http://iec.ch/TC57/CIM100#Pss5.kf) | 1 <br />  float  | Frequency/shaft speed input gain (<i>K</i><i><sub>F</sub></i>) | direct |
| isfreq | [cim:Pss5.isfreq](http://iec.ch/TC57/CIM100#Pss5.isfreq) | 1 <br />  boolean  | Selector for frequency/shaft speed input (<i>isFreq</i>) | direct |
| kpss | [cim:Pss5.kpss](http://iec.ch/TC57/CIM100#Pss5.kpss) | 1 <br />  float  | PSS gain (<i>K</i><i><sub>PSS</sub></i>) | direct |
| ctw2 | [cim:Pss5.ctw2](http://iec.ch/TC57/CIM100#Pss5.ctw2) | 1 <br />  boolean  | Selector for second washout enabling (<i>C</i><i><sub>TW2</sub></i>) | direct |
| tw1 | [cim:Pss5.tw1](http://iec.ch/TC57/CIM100#Pss5.tw1) | 1 <br />  [Seconds](Seconds.md)  | First washout (<i>T</i><i><sub>W1</sub></i>) (&gt;= 0) | direct |
| tw2 | [cim:Pss5.tw2](http://iec.ch/TC57/CIM100#Pss5.tw2) | 1 <br />  [Seconds](Seconds.md)  | Second washout (<i>T</i><i><sub>W2</sub></i>) (&gt;= 0) | direct |
| tl1 | [cim:Pss5.tl1](http://iec.ch/TC57/CIM100#Pss5.tl1) | 1 <br />  [Seconds](Seconds.md)  | Lead/lag time constant (<i>T</i><i><sub>L1</sub></i>) (&gt;= 0) | direct |
| tl2 | [cim:Pss5.tl2](http://iec.ch/TC57/CIM100#Pss5.tl2) | 1 <br />  [Seconds](Seconds.md)  | Lead/lag time constant (<i>T</i><i><sub>L2</sub></i>) (&gt;= 0) | direct |
| tl3 | [cim:Pss5.tl3](http://iec.ch/TC57/CIM100#Pss5.tl3) | 1 <br />  [Seconds](Seconds.md)  | Lead/lag time constant (<i>T</i><i><sub>L3</sub></i>) (&gt;= 0) | direct |
| tl4 | [cim:Pss5.tl4](http://iec.ch/TC57/CIM100#Pss5.tl4) | 1 <br />  [Seconds](Seconds.md)  | Lead/lag time constant (T<sub>L4</sub>) (&gt;= 0) | direct |
| vsmn | [cim:Pss5.vsmn](http://iec.ch/TC57/CIM100#Pss5.vsmn) | 1 <br />  [PU](PU.md)  | Stabilizer output maximum limit (<i>V</i><i><sub>SMN</sub></i>) | direct |
| vsmx | [cim:Pss5.vsmx](http://iec.ch/TC57/CIM100#Pss5.vsmx) | 1 <br />  [PU](PU.md)  | Stabilizer output minimum limit (<i>V</i><i><sub>SMX</sub></i>) | direct |
| tpe | [cim:Pss5.tpe](http://iec.ch/TC57/CIM100#Pss5.tpe) | 1 <br />  [Seconds](Seconds.md)  | Electric power filter time constant (<i>T</i><i><sub>PE</sub></i>) (&gt;= 0) | direct |
| pmin | [cim:Pss5.pmin](http://iec.ch/TC57/CIM100#Pss5.pmin) | 1 <br />  [PU](PU.md)  | Minimum power PSS enabling (<i>Pmin</i>) | direct |
| deadband | [cim:Pss5.deadband](http://iec.ch/TC57/CIM100#Pss5.deadband) | 1 <br />  [PU](PU.md)  | Stabilizer output deadband (<i>DEADBAND</i>) | direct |
| vadat | [cim:Pss5.vadat](http://iec.ch/TC57/CIM100#Pss5.vadat) | 1 <br />  boolean  | <font color="#0f0f0f">Signal selector (<i>V</i><i><sub>adAtt</sub></i>) | direct |
| RemoteInputSignal | [cim:PowerSystemStabilizerDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#PowerSystemStabilizerDynamics.RemoteInputSignal) | * <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this power system stabilizer model | [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md) |
| ExcitationSystemDynamics | [cim:PowerSystemStabilizerDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PowerSystemStabilizerDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power system stabilizer model is asso... | [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md) |
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
| self | cim:Pss5 |
| native | this:Pss5 |




