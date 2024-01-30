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
      
      
      RotatingMachine : IdentifiedObject.description
        
      RotatingMachine : IdentifiedObject.mRID
        
      RotatingMachine : IdentifiedObject.name
        
      RotatingMachine : ConductingEquipment.Terminals
        
          RotatingMachine --> Terminal : ConductingEquipment.Terminals
        
      
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
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RotatingMachine |
| native | this:RotatingMachine |




