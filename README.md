# UE 5.5.4 Learning Project

Well, as the name suggests — this is my learning project, built with Unreal Engine **5.5.4**.

I'm using this space to experiment, try things out, and get a better feel for UE.

## ✅ Current Features

- [x] **3D Camera Orbit**  
  Orbiting around a focus point — smooth and responsive.

- [x] **3D Camera Zoom**  
  Zoom in/out with the scroll wheel using a 10-point linear zoom.  

- [X] **Control Over Camera Focus Point By Navigating Mouse To The Edges Of The Screen**  
  Basic rts camera controll.

- [X] **Camera Focus Point Sticking To Landscape**  
  Based on Line trace, single point, no falling into pits secured by clamp.

## 🛠️ Work in Progress

- [ ] **Click to Move Camera Focus Point To Pointed Destination**  

- [ ] **Minimap**

- [ ] **Camera Sticking Using Event Instead Of Every Tick**🛠️

- [ ] ****

- [ ] **More to Come**  
  One step at a time.

## 🧪 Cool but Unlikely Ideas

These are things that would be awesome to implement one day, but realistically… probably not anytime soon.

- [ ] **More Advanced Camera Sticking**  
  Runtime Virtual Texturing (RVT)/Height map sampling/or multipoint line trace  
(but for now i think most of them are overkill and mutlipoint isn't crucial)
---

## 🔮 Magic System

The magic system is built around a single resource: **mana**, which the hero uses to cast spells during battles.

### 🎯 Core Principles:
- **There are no restrictions during battle** — the player can cast any number of spells as long as they have mana.
- **Mana is logically split into two tiers**:
  - **Fast mana (comfort zone)** – roughly 1/3 of the total pool; regenerates quickly and without penalty.
  - **Remaining mana** – using this causes **exhaustion**, which only affects the hero **after the battle ends**.
- **Exhaustion** slows down mana regeneration between battles or can temporarily lock out strategic map spells (e.g. teleportation).
- The player is **never punished during combat** — the system is built around **strategic decision-making** and long-term resource management.

---

## ✴️ Magic Styles: Chaos and Precision

As part of character development, the player may choose one of two exclusive specialization paths: **Chaos** or **Precision**. Both empower spells, but in very different ways.

### 🔥 Chaos Magic
Style: **raw power, lack of control, instant impact**

- Spells are stronger and cast instantly, but **unpredictable** — they may hit a random target, have side effects, or change behavior mid-cast.
- Best for players who enjoy **risk and spectacle**.
- Often gain bonus effects when cast with low remaining mana.
- Some spells scale with **total mana spent** — e.g. deal damage based on missing mana.

### ❄️ Precision Magic
Style: **planning, preparation, pinpoint accuracy**

- Spells can be **prepared in advance** — they have a delay, but allow **full control** over targeting, timing, and outcome.
- Ideal for players who enjoy **controlling the battlefield**.
- Precision spells often scale with **exact amounts of mana used**, or reward full concentration.
- Some effects may be **ritual-based** — requiring a turn to charge before casting with maximum impact.

> Choosing one path permanently locks the other — the decision is final.

---

## 📖 Spellbook – Interface

The spellbook is visually represented as the **hero opening their hands in a casting gesture**.

- When opened, it displays a **selection of available spells** as icons or glowing sigils floating between the hands.
- Spells are grouped by type:
  - **Neutral** – always available, balanced baseline
  - **Precision** – unlocked only by following the Precision path
  - **Chaos** – unlocked only by following the Chaos path
- The UI allows the player to select a spell and target in a smooth, unified motion.


> It ain't much, but it's honest work.
