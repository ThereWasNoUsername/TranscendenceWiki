# Dynamic Types
Dynamic Types are [Types](Types.md) created during [OnGlobalTypesInit](XML/Type.md#onglobaltypesinit) (via `typCreate`) and [TemplateTypes](XML/TemplateType.md) on game creation, or during gameplay (via `typCreate`).

> The goal of Dymanic Types is to allow an extension to create new types at runtime. For example, this might allow a mod to create a weapon with random properties. As with Betel's suggestion, the way this works is by providing an XML string that describes the type (using all the normal syntax, including embedded code) and adding it as a new type at runtime.

Certain DesignTypes do not support dynamic types.
- AdventureDesc
- Globals
- Image
- Music
- Sound
- EconomyType
- [TemplateType](XML/TemplateType.md)

## On game creation
Dynamic types are initialized after static types are added and before inheritance/overriding/binding occur. There are two ways to create dynamic types.
- [OnGlobalTypesInit](Type.md#onglobaltypesinit)
- [TemplateType](XML/TemplateType.md)

## Post game creation
Certain DesignTypes are not supported after game creation.
- SystemType
- SystemTable
- SystemMap

## References
[Forum post](https://forums.kronosaur.com/viewtopic.php?p=45046#p45046)