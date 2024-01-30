# ValueToAlias


_Describes the translation of one particular value into a name, e.g. 1 as "Open"._





**URI**: [cim:ValueToAlias](http://iec.ch/TC57/CIM100#ValueToAlias)<br />
**Type**: Class




```mermaid
 classDiagram
    class ValueToAlias
      IdentifiedObject <|-- ValueToAlias
      
      ValueToAlias : IdentifiedObject.description
        
      ValueToAlias : IdentifiedObject.mRID
        
      ValueToAlias : IdentifiedObject.name
        
      ValueToAlias : ValueToAlias.value
        
      ValueToAlias : ValueToAlias.ValueAliasSet
        
          ValueToAlias --> ValueAliasSet : ValueToAlias.ValueAliasSet
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **ValueToAlias**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ValueAliasSet | [cim:ValueToAlias.ValueAliasSet](http://iec.ch/TC57/CIM100#ValueToAlias.ValueAliasSet) | 1..1 <br />  [ValueAliasSet](ValueAliasSet.md)  | The ValueAliasSet having the ValueToAlias mappings | direct |
| value | [cim:ValueToAlias.value](http://iec.ch/TC57/CIM100#ValueToAlias.value) | 1..1 <br />  integer  | The value that is mapped | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ValueAliasSet](ValueAliasSet.md) | Values | range | [ValueToAlias](ValueToAlias.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ValueToAlias |
| native | this:ValueToAlias |




