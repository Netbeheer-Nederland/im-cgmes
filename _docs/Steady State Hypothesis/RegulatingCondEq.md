# RegulatingCondEq


_A type of conducting equipment that can regulate a quantity (i.e. voltage or flow) at a specific point in the network._





**URI**: [cim:RegulatingCondEq](http://iec.ch/TC57/CIM100#RegulatingCondEq)<br />
**Type**: Class




```mermaid
 classDiagram
    class RegulatingCondEq
      EnergyConnection <|-- RegulatingCondEq
      

      RegulatingCondEq <|-- ExternalNetworkInjection
      RegulatingCondEq <|-- PowerElectronicsConnection
      RegulatingCondEq <|-- RotatingMachine
      RegulatingCondEq <|-- ShuntCompensator
      RegulatingCondEq <|-- StaticVarCompensator
      
      
      RegulatingCondEq : RegulatingCondEq.controlEnabled
        
      RegulatingCondEq : Equipment.inService
        
      RegulatingCondEq : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * **RegulatingCondEq**
                        * [ExternalNetworkInjection](ExternalNetworkInjection.md)
                        * [PowerElectronicsConnection](PowerElectronicsConnection.md)
                        * [RotatingMachine](RotatingMachine.md)
                        * [ShuntCompensator](ShuntCompensator.md)
                        * [StaticVarCompensator](StaticVarCompensator.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1..1 <br />  boolean  | Specifies the regulation status of the equipment | direct |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1..1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RegulatingCondEq |
| native | this:RegulatingCondEq |




