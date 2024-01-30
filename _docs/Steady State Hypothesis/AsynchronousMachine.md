# AsynchronousMachine


_A rotating machine whose shaft rotates asynchronously with the electrical field.  Also known as an induction machine with no external connection to the rotor windings, e.g. squirrel-cage induction machine._





**URI**: [cim:AsynchronousMachine](http://iec.ch/TC57/CIM100#AsynchronousMachine)<br />
**Type**: Class




```mermaid
 classDiagram
    class AsynchronousMachine
      RotatingMachine <|-- AsynchronousMachine
      
      AsynchronousMachine : AsynchronousMachine.asynchronousMachineType
        
          AsynchronousMachine --> AsynchronousMachineKind : AsynchronousMachine.asynchronousMachineType
        
      AsynchronousMachine : RegulatingCondEq.controlEnabled
        
      AsynchronousMachine : Equipment.inService
        
      AsynchronousMachine : IdentifiedObject.mRID
        
      AsynchronousMachine : RotatingMachine.p
        
          AsynchronousMachine --> ActivePower : RotatingMachine.p
        
      AsynchronousMachine : RotatingMachine.q
        
          AsynchronousMachine --> ReactivePower : RotatingMachine.q
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * [RotatingMachine](RotatingMachine.md)
                            * **AsynchronousMachine**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| asynchronousMachineType | [cim:AsynchronousMachine.asynchronousMachineType](http://iec.ch/TC57/CIM100#AsynchronousMachine.asynchronousMachineType) | 1..1 <br />  [AsynchronousMachineKind](AsynchronousMachineKind.md)  | Indicates the type of Asynchronous Machine (motor or generator) | direct |
| p | [cim:RotatingMachine.p](http://iec.ch/TC57/CIM100#RotatingMachine.p) | 1..1 <br />  [ActivePower](ActivePower.md)  | Active power injection | [RotatingMachine](RotatingMachine.md) |
| q | [cim:RotatingMachine.q](http://iec.ch/TC57/CIM100#RotatingMachine.q) | 1..1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power injection | [RotatingMachine](RotatingMachine.md) |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1..1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1..1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:AsynchronousMachine |
| native | this:AsynchronousMachine |




