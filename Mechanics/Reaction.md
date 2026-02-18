# Reaction

Reaction is an expendable resource. Contrary to Action Points, Reaction Points don't grow with the proficiency level of the hunter — all hunters have **1 Reaction Point** per turn.

## Reaction Points

| Property | Value |
|----------|-------|
| Starting Points | 1 |
| Refresh | Start of each turn |
| Stackable | No (max 1) |

## Uses

Reaction Points can be used for:
1. **Attack of Opportunity** — Make a basic attack when an enemy disengages
2. **Enchantment Triggers** — Activate reactive enchantments (e.g., damage shields, defensive wards)

**Note:** Ability cards do not have Reaction types. Reactions are exclusively for Attacks of Opportunity and enchantment effects.

---

## Attack of Opportunity

An Attack of Opportunity is a reactive strike triggered when an enemy attempts to flee melee combat.

### Triggering Conditions

An Attack of Opportunity is triggered when:

| Condition | Requirement |
|-----------|-------------|
| Engagement | The enemy token is currently engaged with your token (tokens attached) |
| Disengagement | The enemy declares a [[Reposition]] action to move away |
| Reaction Available | You have an unspent Reaction Point |
| Not Surrounded | You are not [[Surrounded]] by enemies |

**Important:** The Attack of Opportunity occurs **before** the enemy completes their reposition. The enemy is still in melee range when the attack is resolved.

### Attack Resolution

Attack of Opportunity uses your **Main Hand weapon stats only**:

**Step 1: Declare Reaction**
- The controlling player declares they will use their Reaction Point
- The disengaging enemy cannot cancel their reposition action

**Step 2: Attack Roll**
```
Attack Roll = 1d20 + Main Hand Attack Bonus
```
Compare against the disengaging enemy's Evasion:
- **Roll ≥ Evasion**: Attack hits, proceed to damage
- **Roll < Evasion**: Attack misses, enemy completes disengagement

**Step 3: Damage Roll**
```
Damage = [Main Hand Weapon Min - Max] - Enemy Armor
```
Roll the weapon's damage die and subtract enemy armor.

**Step 4: Apply Results**
- Apply damage to enemy HP
- Determine injury effects using weapon's [[Injury Traits]]
- Enemy completes their reposition (if still alive and mobile)

### Restrictions

| Restriction | Reason |
|-------------|--------|
| Main Hand Only | Off-hand weapon stats are not used for Attacks of Opportunity |
| Basic Attack Only | No ability cards may be used — only the weapon's basic attack |
| Main Hand Disabled | If the main hand/arm is disabled by injury, cannot make AoO |
| Surrounded | Cannot make Attacks of Opportunity when [[Surrounded]] |
| Reaction Spent | Cannot make AoO if Reaction Point already spent this turn |

### Safe Disengagement

Some abilities allow disengaging **without** triggering Attacks of Opportunity:

| Ability | Effect |
|---------|--------|
| [[Disengaging Kick]] | Kick enemy away, preventing their AoO |
| [[Vanish]] | Disappear before enemy can react |
| [[Smoke Bomb]] | Obscure vision, safe retreat |
| Teleportation | Instant reposition, no trigger |

### Modifiers

Some abilities and stances enhance Attacks of Opportunity:

| Ability | Modifier |
|---------|----------|
| [[Battle Stance]] | +2 Attack Roll, +2 Damage on AoO |
| Reach Weapons | May trigger AoO when enemy enters engagement (see weapon description) |

---

## Enemy Reactions

Enemies also have Reaction Points and can make Attacks of Opportunity:

| Enemy Type | Reaction Points | Notes |
|------------|-----------------|-------|
| Standard | 1 | Most enemies |
| Elite | 1-2 | Defined in stat block |
| Boss | 2+ | Defined in stat block |

**Enemy AoO Resolution:**
- Uses enemy's standard Attack Bonus and Damage as defined in their stat block
- Follows same triggering conditions as hunter AoO
- Cannot make AoO if enemy is [[Surrounded]] or has spent their Reaction Point

---

## Summary Table

| Action | Cost | Trigger | Uses |
|--------|------|---------|------|
| Attack of Opportunity | 1 Reaction | Enemy disengages | Main Hand weapon stats |
| Enchantment Trigger | 1 Reaction | Enchantment-specific | As defined on enchantment |

---

## Related Mechanics

- [[Surrounded]] — Status that prevents Attacks of Opportunity
- [[Reposition]] — The action that triggers disengagement
- [[Injury Traits]] — Determined by weapon used in Attack of Opportunity
- [[Combat]] — Full combat resolution rules