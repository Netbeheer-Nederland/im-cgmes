# WorkLocation


_Information about a particular location for various forms of work._





**URI**: [cim:WorkLocation](http://iec.ch/TC57/CIM100#WorkLocation)<br />
**Type**: Class




```mermaid
 classDiagram
    class WorkLocation
    click WorkLocation href "../WorkLocation"
      Location <|-- WorkLocation
        click Location href "../Location"
      

      WorkLocation <|-- ServiceLocation
        click ServiceLocation href "../ServiceLocation"
      
      
      WorkLocation : Location.CoordinateSystem
        
          WorkLocation --> CoordinateSystem : Location.CoordinateSystem
          click CoordinateSystem href "../CoordinateSystem"
        
      WorkLocation : Location.mainAddress
        
          WorkLocation --> StreetAddress : Location.mainAddress
          click StreetAddress href "../StreetAddress"
        
      WorkLocation : IdentifiedObject.mRID
        
      WorkLocation : IdentifiedObject.name
        
      WorkLocation : Location.PositionPoints
        
          WorkLocation --> PositionPoint : Location.PositionPoints
          click PositionPoint href "../PositionPoint"
        
      WorkLocation : Location.PowerSystemResources
        
          WorkLocation --> PowerSystemResource : Location.PowerSystemResources
          click PowerSystemResource href "../PowerSystemResource"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Location](Location.md)
        * **WorkLocation**
            * [ServiceLocation](ServiceLocation.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| CoordinateSystem | [cim:Location.CoordinateSystem](http://iec.ch/TC57/CIM100#Location.CoordinateSystem) | 1 <br />  [CoordinateSystem](CoordinateSystem.md)  | Coordinate system used to describe position points of this location | [Location](Location.md) |
| mainAddress | [cim:Location.mainAddress](http://iec.ch/TC57/CIM100#Location.mainAddress) | 0..1 <br />  [StreetAddress](StreetAddress.md)  | Main address of the location | [Location](Location.md) |
| PowerSystemResources | [cim:Location.PowerSystemResources](http://iec.ch/TC57/CIM100#Location.PowerSystemResources) | 1 <br />  [PowerSystemResource](PowerSystemResource.md)  | All power system resources at this location | [Location](Location.md) |
| PositionPoints | [cim:Location.PositionPoints](http://iec.ch/TC57/CIM100#Location.PositionPoints) | * <br />  [PositionPoint](PositionPoint.md)  | Sequence of position points describing this location, expressed in coordinate... | [Location](Location.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/GeographicalLocation-EU#Package_GeographicalLocationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WorkLocation |
| native | this:WorkLocation |




