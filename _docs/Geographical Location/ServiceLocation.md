# ServiceLocation


_A real estate location, commonly referred to as premises._





**URI**: [cim:ServiceLocation](http://iec.ch/TC57/CIM100#ServiceLocation)<br />
**Type**: Class




```mermaid
 classDiagram
    class ServiceLocation
      WorkLocation <|-- ServiceLocation
      
      ServiceLocation : Location.CoordinateSystem
        
          ServiceLocation --> CoordinateSystem : Location.CoordinateSystem
        
      ServiceLocation : Location.mainAddress
        
          ServiceLocation --> StreetAddress : Location.mainAddress
        
      ServiceLocation : IdentifiedObject.mRID
        
      ServiceLocation : IdentifiedObject.name
        
      ServiceLocation : Location.PositionPoints
        
          ServiceLocation --> PositionPoint : Location.PositionPoints
        
      ServiceLocation : Location.PowerSystemResources
        
          ServiceLocation --> PowerSystemResource : Location.PowerSystemResources
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Location](Location.md)
        * [WorkLocation](WorkLocation.md)
            * **ServiceLocation**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| CoordinateSystem | [cim:Location.CoordinateSystem](http://iec.ch/TC57/CIM100#Location.CoordinateSystem) | 1..1 <br />  [CoordinateSystem](CoordinateSystem.md)  | Coordinate system used to describe position points of this location | [Location](Location.md) |
| mainAddress | [cim:Location.mainAddress](http://iec.ch/TC57/CIM100#Location.mainAddress) | 0..1 <br />  [StreetAddress](StreetAddress.md)  | Main address of the location | [Location](Location.md) |
| PowerSystemResources | [cim:Location.PowerSystemResources](http://iec.ch/TC57/CIM100#Location.PowerSystemResources) | 1..1 <br />  [PowerSystemResource](PowerSystemResource.md)  | All power system resources at this location | [Location](Location.md) |
| PositionPoints | [cim:Location.PositionPoints](http://iec.ch/TC57/CIM100#Location.PositionPoints) | 0..* <br />  [PositionPoint](PositionPoint.md)  | Sequence of position points describing this location, expressed in coordinate... | [Location](Location.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/GeographicalLocation-EU#Package_GeographicalLocationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ServiceLocation |
| native | this:ServiceLocation |




