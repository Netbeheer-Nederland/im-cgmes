# PowerElectronicsConnection


_A connection to the AC network for energy production or consumption that uses power electronics rather than rotating machines._





**URI**: [cim:PowerElectronicsConnection](http://iec.ch/TC57/CIM100#PowerElectronicsConnection)<br />
**Type**: Class




```mermaid
 classDiagram
    class PowerElectronicsConnection
    click PowerElectronicsConnection href "../PowerElectronicsConnection"
      RegulatingCondEq <|-- PowerElectronicsConnection
        click RegulatingCondEq href "../RegulatingCondEq"
      
      PowerElectronicsConnection : RegulatingCondEq.controlEnabled
        
      PowerElectronicsConnection : Equipment.inService
        
      PowerElectronicsConnection : IdentifiedObject.mRID
        
      PowerElectronicsConnection : PowerElectronicsConnection.p
        
          PowerElectronicsConnection --> ActivePower : PowerElectronicsConnection.p
          click ActivePower href "../ActivePower"
        
      PowerElectronicsConnection : PowerElectronicsConnection.q
        
          PowerElectronicsConnection --> ReactivePower : PowerElectronicsConnection.q
          click ReactivePower href "../ReactivePower"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * **PowerElectronicsConnection**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| p | [cim:PowerElectronicsConnection.p](http://iec.ch/TC57/CIM100#PowerElectronicsConnection.p) | 1 <br />  [ActivePower](ActivePower.md)  | Active power injection | direct |
| q | [cim:PowerElectronicsConnection.q](http://iec.ch/TC57/CIM100#PowerElectronicsConnection.q) | 1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power injection | direct |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PowerElectronicsConnection |
| native | this:PowerElectronicsConnection |




