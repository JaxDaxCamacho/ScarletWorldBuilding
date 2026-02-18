# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an **Obsidian vault** for world-building a deckbuilder adventure game called **Scarlet Obsidian**. It's a turn-based tactical combat game where players control a team of up to 3 Hunters from The Scarlet Company, a mercenary group operating in the Golden Lands continent.

The project uses Obsidian's wikilink format `[[NoteName]]` for internal references between documents.

## Core Game Systems

### Hunters (Player Characters)
Hunters have: Name, Hunter School, Two Discipline Proficiencies, Health State, Injuries, Armor, Weapons (Main/Off hand), Inventory, Portrait, Fame, and Hunter Cards.

### Six Disciplines
Each Hunter can specialize in disciplines that determine their available abilities:
- **Martial** - Melee combat, blocking, weapon skills
- **Subterfuge** - Stealth, backstabs, assassination
- **Survival** - Traps, ranged attacks, environment manipulation
- **Invocation** - Elemental magic (lightning, fire, wind)
- **Metamorphosis** - Alchemy, mutagens, transformations
- **Ecclesiastic** - Divine miracles from The Red God

### Card Types
- **Ability Cards** - Active abilities with Level, AP Cost, Traits, Targets
- **Equipment Cards** - Weapons, armor, shields, trinkets with stats and abilities
- **School Cards** - Permanent enchantments representing hunter training
- **Conjuration Cards** - Summoned creatures/objects
- **Enchantment Cards** - Temporary or permanent buffs/debuffs

## Combat System

### Attack Resolution (6 Steps)
1. **Declare Attack** - Select target, confirm ability
2. **Attack Roll** - `1d20 + Attack Bonus + Modifiers` vs Target Evasion
3. **Damage Roll** - Roll within weapon/ability [min-max] range, add modifiers
4. **Armor Reduction** - `Raw Damage - Target Armor = Damage After Armor`
5. **Apply Resistances** - Immunity (0%), Strong Resistance (50%), Weak Resistance (75%), Vulnerability (150%)
6. **Apply Final Damage** - Subtract from enemy HP, or determine Hunter injury

### Hunter Injuries
Unlike enemies with HP, hunters take injuries based on damage received:
| Damage | Injury |
|--------|--------|
| 1-4 | [[Light injury]] |
| 5-9 | [[Medium Injury]] |
| 10-19 | [[Serious Injury]] |
| 20+ | Death |

The specific injury depends on the attack's **Damage Trait** (see [[Injury Traits]]):
- **Slashing** - Bleeding, mutilations, severed tendons
- **Piercing** - Deep punctures, organ damage
- **Blunt** - Broken bones, concussions
- **Fire/Lightning/Acid/Frost** - Elemental-specific injuries

### Reaction System
All hunters have **1 Reaction Point** per turn (does not stack). Reactions are used for:
- **Attack of Opportunity** - When enemy disengages, spend reaction to make a basic main-hand attack
- **Enchantment Triggers** - Certain enchantments may use reactions

**Attack of Opportunity Rules:**
- Triggered when engaged enemy declares [[Reposition]] to disengage
- Uses main-hand weapon stats only (no ability cards)
- Cannot AoO when [[Surrounded]]
- Enemy must have Reaction Point available

### Positioning & Status
- **Reposition** - 1 AP to engage or disengage with another token
- **Surrounded** - 4+ enemy tokens attached; -4 Evasion, cannot reposition or AoO
- **Engaged** - Tokens attached in melee range
- **Distant** - Not engaged with any enemy

## Directory Structure

| Folder | Purpose |
|--------|---------|
| `Mechanics/` | Core game rules (Combat, Hunter, Enemies, Armor, Reaction, Surrounded, Reposition) |
| `HunterCards/` | Ability cards organized by 6 discipline subfolders |
| `CardTypes/` | Card type definitions and components |
| `Bestiary/` | Enemy/monster definitions |
| `Equipment/` | Weapons and armor items |
| `Injuries/` | Injury type definitions |
| `Campaign/` | Story missions and quests |
| `NPCs/` | Non-player characters |
| `Lore/` | World lore (Fifth Holy Empire, Golden Lands, The Scarlet Company, The Red God) |
| `Schools/` | Hunter school backgrounds |

## Content Conventions

### Card Format (Ability Cards)
```
Level: X
Action Point Cost: X
**Use Weapon Stats** (if applicable - inherits weapon's damage trait)
Abilities:
[Effect description based on target type]
```

### Equipment Format
```
![[image.png]]
Description: [Flavor text]
**Type:** 1 handed / 2 handed
**Damage Trait:** [[Slashing]] / [[Piercing]] / [[Blunt]]
**Attack Bonus:** +X
**Damage:** X-Y
[Basic attack ability]
```

### Enemy Format
```
[Flavor description]
Art![[image.png]]
TokenFrame => [Type]
Size => [Small/Medium/Large/Colossal]
HP => X
Armor => X
Evasion => X
Enemy Abilities => [Ability1, Ability2...]
Enemy Behaviour Type => [AI type]
```

### Wikilinks
All internal references use Obsidian format: `[[NoteName]]`

## Lore Context

The game is set in a dark fantasy world where the **Fifth Holy Empire** has contracted **The Scarlet Company** to clear monsters from the newly discovered **Golden Lands** continent. The primary deity is **The Red God** of fire and sun. Hunters are trained at specialized **Hunter Schools** and are elite monster slayers.