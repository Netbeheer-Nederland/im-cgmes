# CurrentLimit


_Operational limit on current._





**URI**: [cim:CurrentLimit](http://iec.ch/TC57/CIM100#CurrentLimit)<br />
**Type**: Class




```mermaid
 classDiagram
    class CurrentLimit
    click CurrentLimit href "../CurrentLimit"
      OperationalLimit <|-- CurrentLimit
        click OperationalLimit href "../OperationalLimit"
      
      CurrentLimit : IdentifiedObject.mRID
        
      CurrentLimit : CurrentLimit.value
        
          CurrentLimit --> CurrentFlow : CurrentLimit.value
          click CurrentFlow href "../CurrentFlow"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [OperationalLimit](OperationalLimit.md)
        * **CurrentLimit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:CurrentLimit.value](http://iec.ch/TC57/CIM100#CurrentLimit.value) | 1 <br />  [CurrentFlow](CurrentFlow.md)  | Limit on current flow | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CurrentLimit |
| native | this:CurrentLimit |




