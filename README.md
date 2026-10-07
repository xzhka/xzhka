<div align="center">

# Dovbnia Artem

### Junior Unreal Engine C++ Gameplay Programmer

Building gameplay systems with **C++ and Unreal Engine 5**.

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
![Unreal Engine](https://img.shields.io/badge/Unreal%20Engine-313131?style=flat&logo=unrealengine&logoColor=white)
![GAS](https://img.shields.io/badge/GAS-313131?style=flat)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Perforce Helix](https://img.shields.io/badge/PERFORCE%20HELIX-%2300AEEF.svg?style=flat&logo=Perforce&logoColor=white)

**Gameplay Systems · Combat · Multiplayer · Optimization**

</div>

---

## 👋 About Me

Junior Unreal Engine 5 gameplay programmer working in C++. I focus on multiplayer combat systems built on the **Gameplay Ability System (GAS)**, with clean, modular, data-driven code.
I have experience with replication, server-authoritative gameplay, and optimizing with Network Insights, Unreal Insights, and CPU/GPU profiling.
I'm looking for a **junior gameplay programmer** role where I can learn from an experienced team and contribute to shipped titles.

## 🎮 Featured Project

### [FPSCombatSystem](https://github.com/xzhka/FPSCombatSystem)

A multiplayer first-person shooter built in **UE5 C++** on the Gameplay Ability System, using a Lyra-style modular architecture.

**What's inside**

- **Ability system:** Sprint, Dash, Updraft, Reload, Aim, Throw (charge and release), Quickbar switching, and Death, all as GAS abilities on a shared base class. Cooldowns use a SetByCaller pattern, and ability-vs-ability rules live in a Tag Relationship Mapping data asset.
- **Weapons:** A ranged weapon ability with a client-predicted trace and server-side hit validation. Semi, full-auto, and burst fire are separate fire-mode classes. Recoil patterns and spread are data-driven per weapon.
- **Throwables:** A projectile base class configured by data assets, plus an explosive component that applies splash damage through Gameplay Effects.
- **Inventory and equipment:** Item and equipment managers using `FastArraySerializer`, replicated subobjects, and Iris replication fragments.
- **Damage and attributes:** A custom Attribute Set with `Damage` and `Heal` meta attributes, plus damage and heal execution calculations.
- **Game flow:** Death and respawn handled by a custom GameMode (per-player respawn timers).
- **Animation:** C++ anim instances, Linked Anim Layers per weapon, and an IK Rig component that keeps the left hand on the weapon grip.
- **HUD:** Widgets update through the Gameplay Message Subsystem, so UI stays decoupled from gameplay code.

**Project layout**

```
FPSCombatSystem/
├── AbilitySystem/   # base ability, abilities, attribute set, exec calcs, tag relationships
├── Weapons/         # ranged weapon ability, fire modes, projectiles, throwables
├── Equipment/       # equipment manager, quickbar
├── Items/           # item instances and manager (replicated stacks)
├── Characters/      # character, movement, health and stamina components
├── Animation/       # anim instances, IK Rig component
├── Input/           # Enhanced Input config
└── UI/              # HUD widgets
```

**Tech:** Unreal Engine 5 · C++ · GAS · Replication · Enhanced Input · Iris · Gameplay Message Subsystem · Profiling · IK Rig

---

## 🛠️ Technical Focus

| Area | What I work with |
|---|---|
| **Gameplay Ability System** | Custom abilities and base classes, Attribute Sets, Gameplay Effects, execution calculations, gameplay tags, ability tasks, Gameplay Cues |
| **Networking and Replication** | Server-authoritative gameplay, client prediction, replicated properties and structs, `FastArraySerializer`, Server/Client/NetMulticast RPCs, `NetUpdateFrequency` |
| **Architecture** | Lyra-style modular components, data-driven definitions (data assets), decoupled systems via gameplay messages |
| **Character and Combat** | Stats systems, weapons, recoil and spread, projectiles, death and respawn |
| **Animation** | Linked Anim Layers, Aim Offsets, IK Rig |
| **Profiling and Optimization** | Network Insights, Unreal Insights, CPU/GPU profiling |
| **Tools** | Git, Perforce Helix, Visual Studio / Rider, Jira |

---

## 📫 Contact

- 📧 Email: dovbnia.artem.dev@gmail.com
- 💼 LinkedIn: [Artem Dovbnia](https://www.linkedin.com/in/artem-dovbnia-643b82436/)
