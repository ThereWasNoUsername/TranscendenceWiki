# Dynamic Types
Dynamic Types are [Types](Types.md) created during [OnGlobalTypesInit](XML/Type.md#onglobaltypesinit) (via `typCreate`) and [TemplateTypes](XML/TemplateType.md) on game creation, or during gameplay (via `typCreate`)

## On game creation
Dynamic types are initialized after static types are added and before inheritance/overriding/binding occur.

### OnGlobalTypesInit


### TemplateType


## Post game creation
Certain DesignTypes cannot be created after game creation
