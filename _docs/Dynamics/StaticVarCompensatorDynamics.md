# StaticVarCompensatorDynamics


_Static var compensator whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:StaticVarCompensatorDynamics](http://iec.ch/TC57/CIM100#StaticVarCompensatorDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class StaticVarCompensatorDynamics
    click StaticVarCompensatorDynamics href "../StaticVarCompensatorDynamics"
      DynamicsFunctionBlock <|-- StaticVarCompensatorDynamics
        click DynamicsFunctionBlock href "../DynamicsFunctionBlock"
      

      StaticVarCompensatorDynamics <|-- SVCUserDefined
        click SVCUserDefined href "../SVCUserDefined"
      
      
      StaticVarCompensatorDynamics : IdentifiedObject.description
        
      StaticVarCompensatorDynamics : DynamicsFunctionBlock.enabled
        
      StaticVarCompensatorDynamics : IdentifiedObject.mRID
        
      StaticVarCompensatorDynamics : IdentifiedObject.name
        
      StaticVarCompensatorDynamics : StaticVarCompensatorDynamics.StaticVarCompensator
        
          StaticVarCompensatorDynamics --> StaticVarCompensator : StaticVarCompensatorDynamics.StaticVarCompensator
          click StaticVarCompensator href "../StaticVarCompensator"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **StaticVarCompensatorDynamics**
            * [SVCUserDefined](SVCUserDefined.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| StaticVarCompensator | [cim:StaticVarCompensatorDynamics.StaticVarCompensator](http://iec.ch/TC57/CIM100#StaticVarCompensatorDynamics.StaticVarCompensator) | 1 <br />  [StaticVarCompensator](StaticVarCompensator.md)  | Static Var Compensator to which Static Var Compensator dynamics model applies | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [StaticVarCompensator](StaticVarCompensator.md) | StaticVarCompensatorDynamics | range | [StaticVarCompensatorDynamics](StaticVarCompensatorDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:StaticVarCompensatorDynamics |
| native | this:StaticVarCompensatorDynamics |




