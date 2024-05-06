# RotatingMachine


_A rotating machine which may be used as a generator or motor._





**URI**: [cim:RotatingMachine](http://iec.ch/TC57/CIM100#RotatingMachine)<br />
**Type**: Class




```mermaid
 classDiagram
    class RotatingMachine
    click RotatingMachine href "../RotatingMachine"
      RegulatingCondEq <|-- RotatingMachine
        click RegulatingCondEq href "../RegulatingCondEq"
      

      RotatingMachine <|-- AsynchronousMachine
        click AsynchronousMachine href "../AsynchronousMachine"
      RotatingMachine <|-- SynchronousMachine
        click SynchronousMachine href "../SynchronousMachine"
      
      
      RotatingMachine : RegulatingCondEq.controlEnabled
        
      RotatingMachine : Equipment.inService
        
      RotatingMachine : IdentifiedObject.mRID
        
      RotatingMachine : RotatingMachine.p
        
          RotatingMachine --> ActivePower : RotatingMachine.p
          click ActivePower href "../ActivePower"
        
      RotatingMachine : RotatingMachine.q
        
          RotatingMachine --> ReactivePower : RotatingMachine.q
          click ReactivePower href "../ReactivePower"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * **RotatingMachine**
                            * [AsynchronousMachine](AsynchronousMachine.md)
                            * [SynchronousMachine](SynchronousMachine.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| p | [cim:RotatingMachine.p](http://iec.ch/TC57/CIM100#RotatingMachine.p) | 1 <br />  [ActivePower](ActivePower.md)  | Active power injection | direct |
| q | [cim:RotatingMachine.q](http://iec.ch/TC57/CIM100#RotatingMachine.q) | 1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power injection | direct |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RotatingMachine |
| native | this:RotatingMachine |




