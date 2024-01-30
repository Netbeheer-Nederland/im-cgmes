# RotatingMachine


_A rotating machine which may be used as a generator or motor._





**URI**: [cim:RotatingMachine](http://iec.ch/TC57/CIM100#RotatingMachine)<br />
**Type**: Class




```mermaid
 classDiagram
    class RotatingMachine
      RegulatingCondEq <|-- RotatingMachine
      

      RotatingMachine <|-- AsynchronousMachine
      RotatingMachine <|-- SynchronousMachine
      
      
      RotatingMachine : IdentifiedObject.mRID
        
      
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
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RotatingMachine |
| native | this:RotatingMachine |




