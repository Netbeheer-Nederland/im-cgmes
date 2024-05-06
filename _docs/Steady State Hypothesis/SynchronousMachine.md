# SynchronousMachine


_An electromechanical device that operates with shaft rotating synchronously with the network. It is a single machine operating either as a generator or synchronous condenser or pump._





**URI**: [cim:SynchronousMachine](http://iec.ch/TC57/CIM100#SynchronousMachine)<br />
**Type**: Class




```mermaid
 classDiagram
    class SynchronousMachine
    click SynchronousMachine href "../SynchronousMachine"
      RotatingMachine <|-- SynchronousMachine
        click RotatingMachine href "../RotatingMachine"
      
      SynchronousMachine : RegulatingCondEq.controlEnabled
        
      SynchronousMachine : Equipment.inService
        
      SynchronousMachine : IdentifiedObject.mRID
        
      SynchronousMachine : SynchronousMachine.operatingMode
        
          SynchronousMachine --> SynchronousMachineOperatingMode : SynchronousMachine.operatingMode
          click SynchronousMachineOperatingMode href "../SynchronousMachineOperatingMode"
        
      SynchronousMachine : RotatingMachine.p
        
          SynchronousMachine --> ActivePower : RotatingMachine.p
          click ActivePower href "../ActivePower"
        
      SynchronousMachine : RotatingMachine.q
        
          SynchronousMachine --> ReactivePower : RotatingMachine.q
          click ReactivePower href "../ReactivePower"
        
      SynchronousMachine : SynchronousMachine.referencePriority
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * [RotatingMachine](RotatingMachine.md)
                            * **SynchronousMachine**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| operatingMode | [cim:SynchronousMachine.operatingMode](http://iec.ch/TC57/CIM100#SynchronousMachine.operatingMode) | 1 <br />  [SynchronousMachineOperatingMode](SynchronousMachineOperatingMode.md)  | Current mode of operation | direct |
| referencePriority | [cim:SynchronousMachine.referencePriority](http://iec.ch/TC57/CIM100#SynchronousMachine.referencePriority) | 1 <br />  integer  | Priority of unit for use as powerflow voltage phase angle reference bus selec... | direct |
| p | [cim:RotatingMachine.p](http://iec.ch/TC57/CIM100#RotatingMachine.p) | 1 <br />  [ActivePower](ActivePower.md)  | Active power injection | [RotatingMachine](RotatingMachine.md) |
| q | [cim:RotatingMachine.q](http://iec.ch/TC57/CIM100#RotatingMachine.q) | 1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power injection | [RotatingMachine](RotatingMachine.md) |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SynchronousMachine |
| native | this:SynchronousMachine |




