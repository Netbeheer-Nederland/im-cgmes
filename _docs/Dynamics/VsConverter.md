# VsConverter


_DC side of the voltage source converter (VSC)._





**URI**: [cim:VsConverter](http://iec.ch/TC57/CIM100#VsConverter)<br />
**Type**: Class




```mermaid
 classDiagram
    class VsConverter
      ACDCConverter <|-- VsConverter
      
      VsConverter : IdentifiedObject.description
        
      VsConverter : IdentifiedObject.mRID
        
      VsConverter : IdentifiedObject.name
        
      VsConverter : ConductingEquipment.Terminals
        
          VsConverter --> Terminal : ConductingEquipment.Terminals
        
      VsConverter : VsConverter.VSCDynamics
        
          VsConverter --> VSCDynamics : VsConverter.VSCDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [ACDCConverter](ACDCConverter.md)
                    * **VsConverter**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| VSCDynamics | [cim:VsConverter.VSCDynamics](http://iec.ch/TC57/CIM100#VsConverter.VSCDynamics) | 0..1 <br />  [VSCDynamics](VSCDynamics.md)  | Voltage source converter dynamics model used to describe dynamic behaviour of... | direct |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [VSCUserDefined](VSCUserDefined.md) | VsConverter | range | [VsConverter](VsConverter.md) |
| [VSCDynamics](VSCDynamics.md) | VsConverter | range | [VsConverter](VsConverter.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VsConverter |
| native | this:VsConverter |




