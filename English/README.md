# 🧬 DNA in Motion with C. A Simulator to “See” and Feel the World of Single-Strand Polymers

> **Run it in 30 seconds, see it in 1 minute.**
> Random walks, inertial radii, and intuition.

<p align="center">
<img width="1536" height="1024" alt="単鎖ポリマーの世界を“見て”感じるシミュレーター" src="https://github.com/user-attachments/assets/1afde400-3251-45f2-b7c2-d897bab8fd13" />
</p>

---

## Experience (Three Steps Are Enough)

- **Run**: High-speed generation in C (steps × chain length × seed)
- **View**: Output coordinates to PNG/GIF (frames or endpoint diagram)
- **Measure**: Save inertial radius/endpoint distance, etc., to CSV
> The goal is not “understanding” but “reproduction.” Repeatable under identical conditions.

---

## Parameters (Minimal Only)

| Flag               | Meaning            | Default      |
| ----------------- | ------------- | ------- |
| `--steps`         | Total steps         | `10000` |
| `--length`        | Number of beads        | `100`   |
| `--seed`          | Random seed         | `auto`  |
| `--dim`           | Spatial dimension (`2`/`3`) | `3`     |
| `--lattice`       | Lattice walk (on for Z^d)  | `off`   |
| `--self-avoid`    | Self-avoidance (SAW)     | `off`   |
| `--out`           | Output directory      | `./out` |
| `--png` / `--gif` | Visualization format | `--png` |

---

## Output

- trajectory.csv: t,x,y,z
- radius_of_gyration.csv: t,Rg
- end_to_end.csv: t,Ree
- walk.gif / walk_*.png: Visualization

---

## Model and Limitations (Boundaries)

- Default is ideal chain (no interactions)/3D random walk.
- **Self-avoidance** (SAW) handled simply via --self-avoid (rejection/retry scheme).
- Does not account for real DNA charge, stiffness, or solvent effects. Skeletal model for education/introduction.

---

## Applications

- Lecture demos/practicals (seed-fixed for easy answer comparison)
- Building intuition for beginners (iteration between diagrams → equations → data)
- Research prototypes (reusing visualization and metric templates)

---

## License

MIT License

---

## 🧑‍💻 Author

**[Truth Wave ― 真理の波](https://github.com/truthwave)**  
AI tool development and educational tools also available!

## Feel free to contact us
[📩 Inquiries/Quotes](mailto:realmadrid71214591@gmail.com)

---

## 🏁 Final Thoughts

> **Don't embellish. Reproduce.**
> The persuasive power of science lies in the fact that the same conclusions are repeatedly reached.
