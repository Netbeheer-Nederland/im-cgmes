# CSCDynamics


_CSC function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:CSCDynamics](http://iec.ch/TC57/CIM100#CSCDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class CSCDynamics
      HVDCDynamics <|-- CSCDynamics
      

      CSCDynamics <|-- CSCUserDefined
      
      
      CSCDynamics : CSCDynamics.CSConverter
        
          CSCDynamics --> CsConverter : CSCDynamics.CSConverter
        
      CSCDynamics : IdentifiedObject.description
        
      CSCDynamics : DynamicsFunctionBlock.enabled
        
      CSCDynamics : IdentifiedObject.mRID
        
      CSCDynamics : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [HVDCDynamics](HVDCDynamics.md)
            * **CSCDynamics**
                * [CSCUserDefined](CSCUserDefined.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| CSConverter | [cim:CSCDynamics.CSConverter](http://iec.ch/TC57/CIM100#CSCDynamics.CSConverter) | 1..1 <br />  [CsConverter](CsConverter.md)  | Current source converter to which current source converter dynamics model app... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [CsConverter](CsConverter.md) | CSCDynamics | range | [CSCDynamics](CSCDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CSCDynamics |
| native | this:CSCDynamics |




