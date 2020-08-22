# `<TemplateType>`
A TemplateType is a [DesignType](DesignType.md) with an event called [GetTypeSource](TemplateType.md#gettypesource) that runs when types are initialized. A TemplateType is essentially a single dynamic type defined in XML with a guaranteed UNID. 

The easiest way to make a TemplateType is to store some XML source containing replaceable `%fields%` in `<StaticData>` as CDATA, use `typGetStaticData` to retrieve it, and then using `subst` to replace those fields with actual values.

## `<Events>`
For events defined by all DesignTypes, see [Type](Type.md#events)
### `<GetTypeSource>`
This event runs after [OnGlobalTypesInit](Type.md#onglobaltypesinit) on game creation, before inheritance/overriding/binding happen. This means TemplateTypes generate after `OnGlobalTypesInit` dynamic types are added

- Return: String containing an XML source. The game will create a dynamic type with the UNID of enclosing TemplateType.