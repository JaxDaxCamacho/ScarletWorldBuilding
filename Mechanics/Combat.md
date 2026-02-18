Combat is Resolved by turns.
Either the heroes or the enemies go first depending on the encounter initiation (If the party was ambushed etc).

**Reposition** represents movement in the battlefield, any creature that is mobile, can reposition by spending one action point. When it does so it **engages** with another token or **disengages** (if not [[Surrounded]]) with all currently engaged tokens.

 In the Player Turn, the Player Can:

Play Cards from his characters.
Reposition characters (spending one action point).
Interact with [[ObjectTokens]]
End Turn.

In The Enemy Turn:

Each enemy will take decisions on who or what to target with their abilities and do so.
When all enemies are done with actions they end their turn.


---

## Attack Resolution

### Hunter Attacking Enemy

When a hunter performs an Attack Ability against an enemy:

**Step 1: Declare Attack**
- Select target enemy token
- Confirm the attack ability being used
- Determine attack stat source (weapon or ability-specific)

**Step 2: Attack Roll**
```
Attack Roll = 1d20 + Attack Bonus + Modifiers
```

| Modifier | Source |
|----------|--------|
| Effects | Buffs/debuffs on attacker or target |
| Enchantments | Weapon or armor enchantments |
| Injuries | Penalties from active injuries |
| Stances | Combat stance bonuses |
| Positioning | Flanking, high ground, etc. |

**Compare Attack Roll vs Enemy Evasion:**
- **Attack Roll ≥ Enemy Evasion**: Attack hits, proceed to damage
- **Attack Roll < Enemy Evasion**: Attack misses, attack ends

**Step 3: Damage Roll**
```
Base Damage = [Weapon/Ability Min - Max] (roll within range)
```

| Damage Modifier | Calculation |
|-----------------|-------------|
| Base Damage | Roll weapon/ability damage die |
| +/- Modifiers | Add/subtract from effects, stances, enchantments |
| = Total Raw Damage | Sum of all modifiers |

**Step 4: Apply Armor Reduction**
```
Raw Damage - Target Armor = Damage After Armor
```

If Damage After Armor is 0 or negative, no damage is dealt.

**Step 5: Apply Resistances**
Some enemies have trait resistances that further reduce damage:

| Resistance Type | Effect |
|-----------------|--------|
| Immunity | Damage reduced to 0 |
| Resistance (Strong) | Damage reduced by 50% (rounded down) |
| Resistance (Weak) | Damage reduced by 25% (rounded down) |
| Vulnerability | Damage increased by 50% |

```
Damage After Armor × Resistance Multiplier = Final Damage
```

**Step 6: Apply Final Damage**
- Subtract Final Damage from enemy HP
- Enemy may gain injury states as HP decreases
- Trigger any on-hit effects (bleeds, stuns, etc.)

---

### Enemy Attacking Hunter

When an enemy attacks a hunter, the process is similar with additional injury considerations:

**Step 1: Attack Roll**
```
Attack Roll = 1d20 + Enemy Attack Bonus
```

**Ranged Penalty:** Enemy ranged attacks have -2 Attack Bonus.

**Compare vs Hunter Evasion:**
- **Attack Roll ≥ Hunter Evasion**: Attack hits
- **Attack Roll < Hunter Evasion**: Attack misses

**Step 2: Damage Roll**
```
Base Damage = [Enemy Min Damage - Max Damage] (roll within range)
```

**Step 3: Apply Armor Reduction**
```
Raw Damage - Hunter Armor = Damage After Armor
```

**Step 4: Apply Resistances**
Check hunter enchantments or effects for damage resistance:
```
Damage After Armor × Resistance Multiplier = Final Damage
```

**Step 5: Determine Injury**

Hunters do not have HP pools like enemies. Instead, damage translates directly to injuries:

| Final Damage | Injury Severity |
|--------------|-----------------|
| 1-4 | [[Light injury]] |
| 5-9 | [[Medium Injury]] |
| 10-19 | [[Serious Injury]] |
| 20+ | Death |

**Step 6: Apply Injury**
- Roll on appropriate injury table based on attack's damage trait
- Apply injury effects immediately
- Track injury on hunter sheet

---

## Damage Traits & Resistances

### Damage Traits

Each attack has an associated damage trait that determines the type of injury inflicted:

| Trait | Injury Characteristics | Common Sources |
|-------|------------------------|----------------|
| **Slashing** | Bleeding, mutilations, severed tendons | Swords, axes, claws |
| **Piercing** | Deep punctures, organ damage, crippling wounds | Daggers, arrows, spears |
| **Blunt** | Broken bones, concussions, bruising | Hammers, staves, fists |
| **Fire** | Burns, tissue destruction | Fire magic, explosions |
| **Lightning** | Nerve damage, stunning, cardiac effects | Lightning magic |
| **Acid** | Chemical burns, tissue dissolution | Acid attacks, creatures |
| **Frost** | Frostbite, numbness, hypothermia | Ice magic, cold environments |

### Resistance Examples

| Entity | Resistance | Effect |
|--------|------------|--------|
| Fire Elemental | Fire Immunity | Takes 0 fire damage |
| Ice Beast | Frost Resistance (Strong) | Takes 50% frost damage |
| Armored Knight | Slashing Resistance (Weak) | Takes 75% slashing damage |
| Dry Wood Creature | Fire Vulnerability | Takes 150% fire damage |

**Resistance Stacking:** Multiple resistance sources do not stack. Use the strongest applicable resistance.

---

## Injury Traits

The **specific injury** rolled depends on the attack's damage trait. See [[Injury Traits]] for the full trait reference.

When determining injury type:
1. Check the damage source's trait (weapon or ability)
2. Roll on the appropriate injury table for that trait
3. Apply the injury effects immediately

Abilities with "Use Weapon Stats" inherit the weapon's damage trait.



![[CombatSketch.png]]