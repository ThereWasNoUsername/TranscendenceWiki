# Weapon

## Special Damage
### WMD
WMD damage, also known as "mass destruction" or "structural" damage, improves weapon effectiveness against objects with multiple hulls, interior compartments, or non-critical segments. If a weapon has WMD:1 or greater, then the item displays a tag indicating that. Due to implementation details, there are only 8 levels of WMD.

WMD works according to the following table [^1]

| Level | Display tag   | Damage adjust | Kill chance* | 
| ----- | ------------- | ------------- | ------------ |
| WMD:0 | (None)        | 10%           | 2%           |
| WMD:1 | WMD2          | 25%           | 5%           |
| WMD:2 | WMD3          | 32%           | 6.4%         |
| WMD:3 | WMD4          | 40%           | 8%           |
| WMD:4 | WMD5          | 50%           | 10%          |
| WMD:5 | WMD6          | 63%           | 12.6%        |
| WMD:6 | WMD8          | 80%           | 16%          |
| WMD:7 | WMD10         | 100%          | 20%          |

\* Upon damaging a non-critical segment at 0 hp, the target's chance of death is `5% + {WMD kill chance} * {base damage} / {max HP of armor segment}`[^2]

[^1]: [WMD_DATA](https://github.com/kronosaur/TranscendenceDev/blob/ef00d2f7ced0808873c5a1c29e2d5bb4d06a1caa/Mammoth/TSE/Damage.cpp#L116)
[^2]: [iChanceOfDeath](https://github.com/kronosaur/TranscendenceDev/blob/673b6a5ad8d67d09e8c3afd82bdce3ce1fb5e729/Mammoth/TSE/CShip.cpp#L4639)
