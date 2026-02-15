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
- **Ability Cards** - Active abilities with Action Cost, Discipline, Traits, Targets
- **Equipment Cards** - Weapons, armor, shields, trinkets that grant stats and abilities
- **School Cards** - Permanent enchantments representing hunter training
- **Conjuration Cards** - Summoned creatures/objects
- **Enchantment Cards** - Temporary or permanent buffs/debuffs

### Combat System
- **Positioning**: Tokens represent distance - Left/Right/Middle positions, Melee/Distant range
- **Attacks**: Roll 1d20 + Attack Bonus vs Target Evasion
- **Damage**: [min-max] damage minus Armor = Applied Damage
- **Hunter Injuries**: Unlike monsters, hunters take injuries when hit:
  - <5 damage: Light Injury
  - 5-9 damage: Medium Injury (stat penalties)
  - 10-19 damage: Serious Injury (life-threatening)
  - 20+ damage: Death
- **Reposition**: Spend 1 action point to engage/disengage tokens

## Directory Structure

| Folder | Purpose |
|--------|---------|
| `Mechanics/` | Core game rules (Combat, Hunter, Enemies, Armor, etc.) |
| `HunterCards/` | Ability cards organized by discipline subfolders |
| `CardTypes/` | Card type definitions and components |
| `Bestiary/` | Enemy/monster definitions |
| `Equipment/` | Weapons and armor items |
| `Injuries/` | Injury type definitions |
| `Campaign/` | Story missions and quests |
| `NPCs/` | Non-player characters |
| `Lore/` | World lore (Fifth Holy Empire, Golden Lands, The Scarlet Company, The Red God) |
| `Schools/` | Hunter school backgrounds |
| `Side Quest Givers/` | Side quest content |

## Content Conventions

- Card files use Level, Action Point Cost, and ability descriptions
- Enemies have: Name, Description, Art, TokenFrame, Size, Enemy Abilities, Enemy Behaviour Type
- Abilities have: Name, Description, Art, Level, Trait, TargetType, Target Distance, Type, Effect, QTEID
- Links use Obsidian wikilink format: `[[NoteName]]`

## Lore Context

The game is set in a dark fantasy world where the **Fifth Holy Empire** has contracted **The Scarlet Company** to clear monsters from the newly discovered **Golden Lands** continent. The primary deity is **The Red God** of fire and sun. Hunters are trained at specialized **Hunter Schools** and are elite monster slayers.