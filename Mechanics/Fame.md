# Fame & Infamy

Fame and Infamy represent the hunter's reputation throughout the Golden Lands. This is a single tracked resource measured on a scale from -100 to +100.

```
INFAMY ←―――――――― 0 ――――――――→ FAME
   -100 ... -50 ... 0 ... +50 ... +100
```

## Reputation Tiers

| Tier | Range | Status | Description |
|------|-------|--------|-------------|
| **Hero** | +80 to +100 | Legendary | Songs are sung about this hunter. NPCs seek them out. |
| **Renowned** | +50 to +79 | Famous | Well-known across settlements. Unlocks diplomatic options. |
| **Respected** | +20 to +49 | Known | Good reputation, minor benefits with NPCs. |
| **Neutral** | -19 to +19 | Unknown | No reputation effects. New hunters start here. |
| **Questioned** | -20 to -49 | Suspicious | NPCs are wary. Some merchants charge more. |
| **Feared** | -50 to -79 | Infamous | Name spoken in whispers. Unlocks intimidation options. |
| **Notorious** | -80 to -100 | Dreaded | Even criminals give this hunter wide berth. |

---

## Fame Effects

### Dialogue Options
Fame unlocks additional dialogue choices during multi-option interactions:

| Fame Threshold | Unlocks |
|----------------|---------|
| +20 | "I've helped people like you before..." (Persuasion bonus) |
| +40 | "Perhaps we can find a peaceful solution." (Diplomatic option) |
| +60 | "I'm here on behalf of the settlement." (Authority option) |
| +80 | "The people trust my judgment." (Leadership option) |

### Action Options
| Fame Threshold | Unlocks |
|----------------|---------|
| +30 | Request free lodging at inns |
| +50 | Request supplies from settlement leaders |
| +70 | Recruit temporary allies without payment |

### Merchant Benefits
| Fame Threshold | Effect |
|----------------|--------|
| +25 | 10% discount on purchases |
| +50 | 15% discount, access to rare items |
| +75 | 25% discount, first pick of new stock |

---

## Infamy Effects

### Dialogue Options
Infamy unlocks darker dialogue choices:

| Infamy Threshold | Unlocks |
|------------------|---------|
| -20 | "You really want to test me?" (Intimidation) |
| -40 | "I've killed people for less." (Threat option) |
| -60 | "One word and you're dead." (Lethal threat) |
| -80 | "I am the nightmare you fear." (Terror option) |

### Action Options
| Infamy Threshold | Unlocks |
|------------------|---------|
| -30 | Intimidate NPCs for free information |
| -50 | Threaten merchants for discounts |
| -70 | Force surrendered enemies to flee without combat |

### Consequences
| Infamy Threshold | Effect |
|------------------|--------|
| -25 | Some shops refuse service |
| -50 | Guards watch the hunter closely |
| -75 | Bounty hunters may track the hunter |

---

## Reputation Changes

### Gaining Fame (+)
| Action | Fame Change |
|--------|-------------|
| Complete contract honorably | +3 to +10 |
| Protect civilians | +5 |
| Spare surrendered enemy | +2 |
| Help settlement | +5 to +15 |
| Refuse immoral contract | +5 |
| Return stolen goods | +3 |

### Gaining Infamy (-)
| Action | Infamy Change |
|--------|---------------|
| Complete contract ruthlessly | -3 to -10 |
| Kill civilian or innocent | -15 |
| Kill surrendered enemy | -5 |
| Intimidate innocent NPC | -3 |
| Break agreement or contract | -10 |
| Loot from allies | -5 |

---

## Mixed Reputation Interactions

Some NPCs and factions respond differently to Fame and Infamy:

| NPC Type | Prefers | Dislikes |
|----------|---------|----------|
| Settlement Leaders | Fame (+) | Infamy (-) |
| Merchants | Fame (+) | Neutral |
| Criminals | Infamy (-) | Fame (+) |
| Mercenaries | Either | Neutral |
| The Scarlet Company | Neutral | Extreme Infamy (-80) |
| Religious Figures | Fame (+) | Infamy (-) |

---

## Starting Value

New hunters begin at **0 (Neutral)** — an unknown mercenary with no reputation.

---

## Related Mechanics

- [[Resources]] — Complete resource system including Escudos and Supplies
- [[Character Creation]] — Starting values for new hunters
- [[Campaign]] — Contracts and reputation rewards