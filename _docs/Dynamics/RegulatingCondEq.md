# RegulatingCondEq


_A type of conducting equipment that can regulate a quantity (i.e. voltage or flow) at a specific point in the network._





**URI**: [cim:RegulatingCondEq](http://iec.ch/TC57/CIM100#RegulatingCondEq)<br />
**Type**: Class




```mermaid
 classDiagram
    class RegulatingCondEq
    click RegulatingCondEq href "../RegulatingCondEq"
      EnergyConnection <|-- RegulatingCondEq
        click EnergyConnection href "../EnergyConnection"
      

      RegulatingCondEq <|-- PowerElectronicsConnection
        click PowerElectronicsConnection href "../PowerElectronicsConnection"
      RegulatingCondEq <|-- RotatingMachine
        click RotatingMachine href "../RotatingMachine"
      RegulatingCondEq <|-- StaticVarCompensator
        click StaticVarCompensator href "../StaticVarCompensator"
      
      
      RegulatingCondEq : IdentifiedObject.description
        
      RegulatingCondEq : IdentifiedObject.mRID
        
      RegulatingCondEq : IdentifiedObject.name
        
      RegulatingCondEq : ConductingEquipment.Terminals
        
          RegulatingCondEq --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * **RegulatingCondEq**
                        * [PowerElectronicsConnection](PowerElectronicsConnection.md)
                        * [RotatingMachine](RotatingMachine.md)
                        * [StaticVarCompensator](StaticVarCompensator.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | * <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RegulatingCondEq |
| native | this:RegulatingCondEq |




