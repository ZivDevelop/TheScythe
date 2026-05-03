#TheScythe: Hybrid Combat System
Welcome to the abyss. TheScythe is a high-octane action prototype developed in Unreal Engine 5, focusing on a complex "Scythe-Hybrid" character. This project showcases advanced blueprint logic, multi-layered movement systems, and intelligent NPC combat behaviors.
As a Hybrid entity, the player isn't just a tank with 10,000 HP—they are a precision instrument of destruction.

Adaptive Health System: Custom Damage Logic and real-time HP bar synchronization.

The Abyssal Charge (Right-Click):

Phase 1: Charging state with procedural Screen Shake.

Phase 2 (The Mark): A dynamic UI system scans the target.

💀 Skull with X: Target exceeds execution threshold.

💀 Pure Skull: Target is ready for the end.

Phase 3 (Blink Execution): After a 2-second charge, the player teleports behind the opponent, dealing massive, scaled damage.

Kinetic Movement Gimmick
The movement isn't just "WASD". It’s a layered system designed for flow:

State 1 (Walk): Precision movement.

State 2 (Run): Standard traversal.

State 3 (Fast Run): Activated via a "Press once, then Hold" Shift key mechanic. This requires specific input-buffer logic to differentiate between a tap and a sustained sprint.
The enemies in this world are relentless. They don't just stand there; they hunt.

Seek & Destroy: NPCs use a constant pursuit logic to close the gap with the player.

Proximity-Based Combat:

Once the player is within a specific radius, the AI triggers an Attack Animation.

Hitbox Verification: Every swing is checked via a frame-perfect collision system. If the scythe (or enemy weapon) connects, the damage logic is applied.

Death States: Fully implemented death logic where enemies transition from active threats to static ragdolls/corpses upon health depletion.
Engine: Unreal Engine 5.3+

Language: Blueprints (with C++ optimized headers)

Physics: Custom Hitbox Collision & Trace-based damage.

UI/UX: Dynamic progress bars and conditional icon rendering based on enemy health states.
Developed by ZivDevelop as part of a deep dive into UE5 combat systems.
