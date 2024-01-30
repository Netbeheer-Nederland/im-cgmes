# ApparentPowerLimit


_Apparent power limit._





**URI**: [cim:ApparentPowerLimit](http://iec.ch/TC57/CIM100#ApparentPowerLimit)<br />
**Type**: Class




```mermaid
 classDiagram
    class ApparentPowerLimit
      OperationalLimit <|-- ApparentPowerLimit
      
      ApparentPowerLimit : IdentifiedObject.mRID
        
      ApparentPowerLimit : ApparentPowerLimit.value
        
          ApparentPowerLimit --> ApparentPower : ApparentPowerLimit.value
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [OperationalLimit](OperationalLimit.md)
        * **ApparentPowerLimit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| value | [cim:ApparentPowerLimit.value](http://iec.ch/TC57/CIM100#ApparentPowerLimit.value) | 1..1 <br />  [ApparentPower](ApparentPower.md)  | The apparent power limit | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ApparentPowerLimit |
| native | this:ApparentPowerLimit |




