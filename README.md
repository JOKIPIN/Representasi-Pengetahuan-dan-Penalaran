# 🧠 Semantic Network and Frame Representation

This project demonstrates the use of **Semantic Networks** and **Frame Representation** to model relationships between various entities in the animal kingdom. We visualize an extended **semantic network** using **NetworkX** and **Matplotlib**. Additionally, key entities are structured using **Frame Representation**.

## 📊 Jaringan Semantik yang Diperluas

In this extended semantic network, we explore relationships between animals, their characteristics, habitats, and food sources. The graph provides an intuitive way to represent how these elements are connected.

### 📈 Network Visualization

![Extended Semantic Network](your-image-url-here)

In this semantic network:
- **Red nodes** highlight important entities like "Ayam", "Unggas", and "Biji-bijian".
- **Green edge labels** represent relationships such as `ISA` (is-a), `HAS-PART` (part-of), and `Makan` (eats).

### 🔗 Key Nodes and Edges
- **Nodes**: 
    - Represent entities like animals, habitats, food sources, etc.
    - Examples: "Ayam", "Penguin", "Peternakan", "Krill", "Antartika".
- **Edges**: 
    - Define relationships between the nodes.
    - Examples: `ISA` (is-a), `HAS-PART` (has part), `Makan` (eats), `Habitat` (lives in).

### 🌐 Node and Relationship Highlights
| **Node**            | **Description**                |
|---------------------|--------------------------------|
| **Ayam**            | A type of bird (Unggas) that eats grains. |
| **Penguin**         | A bird that cannot fly, lives in cold habitats. |
| **Burung Hantu**    | A bird that eats small mammals and insects. |
| **Habitat**         | Describes where animals live, e.g., "Hutan", "Antartika". |

| **Relationship**     | **Description**                |
|----------------------|--------------------------------|
| **ISA**              | Defines a hierarchical relationship (e.g., "Unggas" `ISA` "Hewan"). |
| **HAS-PART**         | Indicates part-whole relationship (e.g., "Ayam" `HAS-PART` "Kaki"). |
| **Makan**            | Describes what an entity eats (e.g., "Ayam" `Makan` "Biji-bijian"). |
| **Habitat**          | Describes the habitat of an entity (e.g., "Penguin" `Habitat` "Antartika"). |

---

## 🛠️ Frame Representation

Frames are used to represent complex entities and their attributes in a structured format. Below are some key **frames** that describe objects like animals, their parts, and behaviors.

### 🎯 Frame Definitions

The following table provides details of the **frames** created for different entities in the semantic network.

| **Frame Name**  | **Attributes (Slots)**           | **Description**                               |
|-----------------|----------------------------------|-----------------------------------------------|
| **Animal**      | `ISA`: LivingBeing               | Defines all living beings.                    |
| **Mammal**      | `ISA`: Animal, `HAS-PART`: tail  | Describes mammals, a subclass of animals.     |
| **Cat**         | `ISA`: Mammal, `HAS-PART`: tail, `EATS`: Cat food, `INST`: Garfield, Sylvester | Defines characteristics of cats. |
| **Garfield**    | `ISA`: Cat, `EATS`: Lasagna      | Garfield is a famous instance of a cat.       |
| **Bird**        | `ISA`: Animal, `HAS-PART`: wing, feather, `EATS`: Seeds, `CAN`: Fly | Describes birds, their body parts, and food. |
| **Canary**      | `ISA`: Bird, `EATS`: Seeds, `INST`: Tweety | A specific bird type that eats seeds.         |
| **Penguin**     | `ISA`: Bird, `CANNOT`: Fly, `INST`: Opus | Penguins cannot fly, a specific bird species. |
| **Tweety**      | `ISA`: Canary                   | Tweety is a famous canary.                    |
| **Opus**        | `ISA`: Penguin                  | Opus is a famous penguin.                     |

---

### 🗂️ Detailed Frame Examples

Here is a breakdown of some frames and their attributes:

#### 🐱 Cat Frame
| **Slot**  | **Filler**          |
|-----------|---------------------|
| `ISA`     | Mammal              |
| `HAS-PART`| tail                |
| `EATS`    | Cat food            |
| `INST`    | Garfield, Sylvester |

This frame describes **Cat** as a type of **Mammal**, which has a tail and eats cat food. Famous instances include **Garfield** and **Sylvester**.

#### 🐧 Penguin Frame
| **Slot**  | **Filler**          |
|-----------|---------------------|
| `ISA`     | Bird                |
| `CANNOT`  | Fly                 |
| `INST`    | Opus                |

Penguins are defined as a type of bird that **cannot** fly. An example of a famous penguin is **Opus**.

---

## 🚀 How to Run the Project

1. **Clone this repository**:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2. **Install the dependencies**:
    ```bash
    pip install matplotlib networkx
    ```
3. **Run the script** to visualize the semantic network and display frame information:
    ```bash
    python semantic_network.py
    ```

---

## 📚 Conclusion

This project showcases how **Semantic Networks** and **Frames** can be effectively used to model knowledge domains. The semantic network offers an intuitive visual representation of entities and their relationships, while frames provide a structured and detailed description of each object and its attributes.

Feel free to explore and extend the network by adding more entities, relationships, and frames!
