# ValueAliasSet


_Describes the translation of a set of values into a name and is intendend to facilitate custom translations. Each ValueAliasSet has a name, description etc. A specific Measurement may represent a discrete state like Open, Closed, Intermediate etc. This requires a translation from the MeasurementValue.value number to a string, e.g. 0-&gt;"Invalid", 1-&gt;"Open", 2-&gt;"Closed", 3-&gt;"Intermediate". Each ValueToAlias member in ValueAliasSet.Value describe a mapping for one particular value to a name._





**URI**: [cim:ValueAliasSet](http://iec.ch/TC57/CIM100#ValueAliasSet)<br />
**Type**: Class




```mermaid
 classDiagram
    class ValueAliasSet
      IdentifiedObject <|-- ValueAliasSet
      
      ValueAliasSet : ValueAliasSet.Commands
        
          ValueAliasSet --> Command : ValueAliasSet.Commands
        
      ValueAliasSet : IdentifiedObject.description
        
      ValueAliasSet : ValueAliasSet.Discretes
        
          ValueAliasSet --> Discrete : ValueAliasSet.Discretes
        
      ValueAliasSet : IdentifiedObject.mRID
        
      ValueAliasSet : IdentifiedObject.name
        
      ValueAliasSet : ValueAliasSet.RaiseLowerCommands
        
          ValueAliasSet --> RaiseLowerCommand : ValueAliasSet.RaiseLowerCommands
        
      ValueAliasSet : ValueAliasSet.Values
        
          ValueAliasSet --> ValueToAlias : ValueAliasSet.Values
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **ValueAliasSet**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Commands | [cim:ValueAliasSet.Commands](http://iec.ch/TC57/CIM100#ValueAliasSet.Commands) | 0..* <br />  [Command](Command.md)  | The Commands using the set for translation | direct |
| Discretes | [cim:ValueAliasSet.Discretes](http://iec.ch/TC57/CIM100#ValueAliasSet.Discretes) | 0..* <br />  [Discrete](Discrete.md)  | The Measurements using the set for translation | direct |
| RaiseLowerCommands | [cim:ValueAliasSet.RaiseLowerCommands](http://iec.ch/TC57/CIM100#ValueAliasSet.RaiseLowerCommands) | 0..* <br />  [RaiseLowerCommand](RaiseLowerCommand.md)  | The Commands using the set for translation | direct |
| Values | [cim:ValueAliasSet.Values](http://iec.ch/TC57/CIM100#ValueAliasSet.Values) | 1..* <br />  [ValueToAlias](ValueToAlias.md)  | The ValueToAlias mappings included in the set | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Command](Command.md) | ValueAliasSet | range | [ValueAliasSet](ValueAliasSet.md) |
| [Discrete](Discrete.md) | ValueAliasSet | range | [ValueAliasSet](ValueAliasSet.md) |
| [RaiseLowerCommand](RaiseLowerCommand.md) | ValueAliasSet | range | [ValueAliasSet](ValueAliasSet.md) |
| [ValueToAlias](ValueToAlias.md) | ValueAliasSet | range | [ValueAliasSet](ValueAliasSet.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ValueAliasSet |
| native | this:ValueAliasSet |




