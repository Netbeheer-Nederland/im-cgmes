# VSCUserDefined


_Voltage source converter (VSC) function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:VSCUserDefined](http://iec.ch/TC57/CIM100#VSCUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class VSCUserDefined
      VSCDynamics <|-- VSCUserDefined
      
      VSCUserDefined : IdentifiedObject.description
        
      VSCUserDefined : DynamicsFunctionBlock.enabled
        
      VSCUserDefined : IdentifiedObject.mRID
        
      VSCUserDefined : IdentifiedObject.name
        
      VSCUserDefined : VSCUserDefined.proprietary
        
      VSCUserDefined : VSCUserDefined.ProprietaryParameterDynamics
        
          VSCUserDefined --> ProprietaryParameterDynamics : VSCUserDefined.ProprietaryParameterDynamics
        
      VSCUserDefined : VSCDynamics.VsConverter
        
          VSCUserDefined --> VsConverter : VSCDynamics.VsConverter
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [HVDCDynamics](HVDCDynamics.md)
            * [VSCDynamics](VSCDynamics.md)
                * **VSCUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:VSCUserDefined.proprietary](http://iec.ch/TC57/CIM100#VSCUserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:VSCUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#VSCUserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| VsConverter | [cim:VSCDynamics.VsConverter](http://iec.ch/TC57/CIM100#VSCDynamics.VsConverter) | 1..1 <br />  [VsConverter](VsConverter.md)  | Voltage source converter to which voltage source converter dynamics model app... | [VSCDynamics](VSCDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | VSCUserDefined | range | [VSCUserDefined](VSCUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VSCUserDefined |
| native | this:VSCUserDefined |




