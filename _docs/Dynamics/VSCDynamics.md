# VSCDynamics


_VSC function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:VSCDynamics](http://iec.ch/TC57/CIM100#VSCDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class VSCDynamics
    click VSCDynamics href "../VSCDynamics"
      HVDCDynamics <|-- VSCDynamics
        click HVDCDynamics href "../HVDCDynamics"
      

      VSCDynamics <|-- VSCUserDefined
        click VSCUserDefined href "../VSCUserDefined"
      
      
      VSCDynamics : IdentifiedObject.description
        
      VSCDynamics : DynamicsFunctionBlock.enabled
        
      VSCDynamics : IdentifiedObject.mRID
        
      VSCDynamics : IdentifiedObject.name
        
      VSCDynamics : VSCDynamics.VsConverter
        
          VSCDynamics --> VsConverter : VSCDynamics.VsConverter
          click VsConverter href "../VsConverter"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [HVDCDynamics](HVDCDynamics.md)
            * **VSCDynamics**
                * [VSCUserDefined](VSCUserDefined.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| VsConverter | [cim:VSCDynamics.VsConverter](http://iec.ch/TC57/CIM100#VSCDynamics.VsConverter) | 1 <br />  [VsConverter](VsConverter.md)  | Voltage source converter to which voltage source converter dynamics model app... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [VsConverter](VsConverter.md) | VSCDynamics | range | [VSCDynamics](VSCDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VSCDynamics |
| native | this:VSCDynamics |




