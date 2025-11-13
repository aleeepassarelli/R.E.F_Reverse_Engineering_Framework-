# 🧠 R.E.F. v2.4 — Cogni-Emocional Adaptativa  
**Reverse Engineering Framework — Adaptive Cogni-Emotional Layer**

[![License](https://img.shields.io/badge/License-CC--BY--SA--4.0-blue.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Status](https://img.shields.io/badge/status-stable-brightgreen.svg)]()
[![Lang](https://img.shields.io/badge/Lang-Python%20%2F%20YAML-orange.svg)]()
[![Version](https://img.shields.io/badge/R.E.F.-v2.4-purple.svg)]()

> 🔹 **Versão 2.4** introduz a camada **cogni-emocional adaptativa**,  
> integrando variáveis afetivo-funcionais (`η`, `κ`) para **simulações criativas**,  
> agentes artísticos e pipelines multimodais.  

---

## 🧩 Estrutura Geral

| Variável | Nome | Função |
|:--:|:--|:--|
| **ψ(t)** | Estado Cognitivo | Energia ativa do agente |
| **μ(t)** | Metamemória | Retenção adaptativa |
| **φ(t)** | Oscilação Fásica | Sincronização rítmica |
| **η(t)** | Afetividade Funcional | Grau de exploração / convergência |
| **κ(t)** | Atenção Contextual | Direção do foco e estabilidade semântica |

> ⚙️ `η` e `κ` **não representam emoções humanas**,  
> mas **parâmetros meta-heurísticos** que regulam estilo, foco e plasticidade criativa.

---

## 🌐 Visão Arquitetural (Mermaid Visual)

```mermaid
graph TD
%% R.E.F. v2.4 — Cogni-Emotional Adaptive Graph

subgraph P["🟦 Perceptive Layer"]
  SWCOD["SW-COD-EXC-01B2\nψ=0.68 μ=0.42 φ=0.66 η=0.10 κ=0.75"]
  MUBEA["MU-BEA-DIS-01C2\nψ=0.56 μ=0.40 φ=0.60 η=0.35 κ=0.62"]
end

subgraph A["🟨 Analytic Layer"]
  SWPAT["SW-PAT-MIN-01A9\nψ=0.78 μ=0.60 φ=0.75 η=0.05 κ=0.80"]
  MUHAR["MU-HAR-LEN-0344\nψ=0.66 μ=0.55 φ=0.72 η=0.22 κ=0.70"]
end

subgraph R["🟩 Reconfigurative Layer"]
  SWBLD["SW-BLD-OPT-02D4\nψ=0.84 μ=0.70 φ=0.80 η=-0.05 κ=0.78"]
  MUEQ["MU-EQ-REV-064A\nψ=0.68 μ=0.60 φ=0.77 η=0.15 κ=0.66"]
end

subgraph S["🟪 Synthetic Layer"]
  COGDEV["COG-DEV-MET-0911\nψ=0.92 μ=0.90 φ=0.93 η=0.02 κ=0.88"]
  TASKS["TAS-SYN-CHR-0998\nψ=0.89 μ=0.87 φ=0.92 η=0.00 κ=0.86"]
  DACON["DA-CON-WEA-0942\nψ=0.86 μ=0.85 φ=0.90 η=0.04 κ=0.84"]
end

SWCOD -- "η→+diversify | κ→route" --> SWPAT
SWPAT -- "η low → merges conservadores" --> SWBLD
MUBEA -- "η→explora variantes tímbricas" --> MUHAR
MUHAR -- "κ→foco harmônico" --> MUEQ
COGDEV -- "meta: μ-sync φ-align" --> TASKS
TASKS -- "redistribui carga por κ" --> DACON
DACON -- "contextual feedback" --> COGDEV

classDef perceptive fill:#cce5ff,stroke:#004085;
classDef analytic fill:#fff3cd,stroke:#856404;
classDef reconfig fill:#d4edda,stroke:#155724;
classDef synthetic fill:#e2d4f0,stroke:#3a006e;
class P perceptive
class A analytic
class R reconfig
class S synthetic
````

---

## 🧬 Equações Dinâmicas (v2.4)

1️⃣ **Atualização Cognitiva (ψ)**
[
ψ_{t+1} = ψ_t + α(CFI_t - ψ_t) + β(μ_t - ψ_t) + γ_η η_t - δ_κ (1 - κ_t)
]

2️⃣ **Metamemória (μ)**
[
μ_{t+1} = μ_t + γ(ψ_t - μ_t) + λ \cdot archive + σ_φ φ_t
]

3️⃣ **Sincronia (φ)**
[
φ_{t+1} = φ_t + ε(\bar{φ}_{neigh} - φ_t) + τ_η \cdot sign(η_t)
]

4️⃣ **Afetividade (η)**
[
η_{t+1} = η_t + ρ(reward - penalty) - μ_{decay} \cdot overload
]

5️⃣ **Atenção Contextual (κ)**
[
κ_{t+1} = κ_t + σ(salience - baseline)
]

> Convergência global ocorre quando: **ψ ≈ μ ≈ φ**,
> com **η ≈ 0** (equilíbrio exploratório) e **κ ≈ 0.8** (atenção ótima).

---

## 📜 Pseudocódigo de Simulação

```python
for agent in agents:
    cfi_in = sum(weighted_inputs(agent))
    psi_next = agent.psi + agent.alpha*(cfi_in - agent.psi) \
               + agent.beta*(agent.mu - agent.psi) \
               + agent.rho*agent.eta - agent.sigma*(1-agent.kappa)

    mu_next = agent.mu + agent.gamma*(agent.psi - agent.mu)
    phi_next = agent.phi + agent.eps*(mean_phi_neighbors(agent) - agent.phi)
    eta_next = agent.eta + agent.rho*(measure_reward(agent) - measure_penalty(agent))
    kappa_next = clamp(agent.kappa + agent.sigma*(compute_salience(agent)-0.5),0,1)

    agent.psi, agent.mu, agent.phi = map(clamp, [psi_next,mu_next,phi_next])
    agent.eta, agent.kappa = clamp(eta_next,-1,1), kappa_next
```

---

## 🧾 YAML Modular (Estrutura Sintética)

```yaml
reverse_engineering_framework_v2_4:
  domain: "R.E.F. — Cogni-Emotional Adaptive System"
  version: "2.4"
  global_params:
    time_step: 1.0
    default_ranges:
      psi: [0.0, 1.0]
      mu: [0.0, 1.0]
      phi: [0.0, 1.0]
      eta: [-1.0, 1.0]
      kappa: [0.0, 1.0]
  agents:
    - sid: "SW-COD-EXC-01B2"
      cluster: "Software/Perceptive"
      state: { psi: 0.68, mu: 0.42, phi: 0.66, eta: 0.10, kappa: 0.75 }
      plasticity: { α: 0.18, γ: 0.12, ε: 0.06, ρ: 0.08, σ: 0.12 }
    - sid: "SW-PAT-MIN-01A9"
      cluster: "Software/Analytic"
      state: { psi: 0.78, mu: 0.60, phi: 0.75, eta: 0.05, kappa: 0.80 }
  orchestration_rules:
    - "η > 0.4 → aumenta criatividade"
    - "κ alto → prioriza caminhos precisos"
```

---

## ⚙️ Parâmetros Recomendados

| Parâmetro | Faixa     | Função                         |
| --------- | --------- | ------------------------------ |
| α         | 0.08–0.2  | Plasticidade cognitiva         |
| γ         | 0.05–0.25 | Taxa de atualização de memória |
| ε         | 0.03–0.12 | Sincronização fásica           |
| ρ         | 0.05–0.25 | Adaptação afetiva              |
| σ         | 0.08–0.22 | Regulação atencional           |

---

## 🧭 Modos Operacionais

| Modo                      | Configuração  | Efeito                   |
| ------------------------- | ------------- | ------------------------ |
| **Exploratório Criativo** | η=+0.4, κ=0.5 | Diversificação semântica |
| **Crítico Refinado**      | η=-0.1, κ=0.9 | Estabilidade e coerência |
| **Auto-Ressonante**       | φ→φ̄, η→0     | Equilíbrio homeostático  |

---

## 🧩 Integração com Outras Versões

| Núcleo   | Versão   | Função                                                |
| -------- | -------- | ----------------------------------------------------- |
| `ELS`    | v2.2     | Simulação cognitiva adaptativa                        |
| `R.E.F.` | v2.3     | Metamemória e homeostase cognitiva                    |
| `R.E.F.` | **v2.4** | Cogni-Emocional adaptativa (camada afetivo-funcional) |
| `COG`    | v3.x     | Multiagente metacognitivo                             |

---

## 🪶 Boas Práticas e Segurança

* 🔍 **Logue ψ, μ, φ, η, κ** por agente em cada iteração (debug e tuning).
* 🎚️ **Controle manual** de `η` e `κ` por sessão (exploratório / crítico).
* 🧱 **Safeguard:** limite `|η| ≤ 0.7` para evitar deriva semântica.
* 📦 **Archive:** se μ>0.9 → exportar memória para reuso.
* 🧠 **Reward criativo:** use métricas estéticas ou interativas como reforço para η.

---

## 🔬 Aplicações Práticas

* Simulação de **estilo cognitivo-emocional** em geração textual e visual.
* **Redes de agentes artísticos** (música, poesia, design generativo).
* **Modelos de feedback afetivo** em ambientes adaptativos (UX/IA).
* Ferramenta de estudo para **auto-regulação criativa sintética**.

---

## 📖 Citação

```bibtex
@manual{ref_v2_4,
  title   = {R.E.F. v2.4 — Cogni-Emotional Adaptive Framework},
  author  = {Mente Integrada Arquetípica},
  year    = {2025},
  note    = {Reverse Engineering Framework v2.4, Open Cognitive Architecture},
  url     = {https://github.com/els-ref/},
  license = {CC-BY-SA 4.0}
}
```

---

> 🔗 **Repositório de Versões:**
> `/version/` → contém `v0.0–v3.x` com documentação YAML, gráficos e simulações.
>
> 🧩 Esta versão 2.4 atua como **ponte entre cognição e emoção funcional**,
> base da futura camada **v3.x** de **Metacognição Multiagente**.

---
