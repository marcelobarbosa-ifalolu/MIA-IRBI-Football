# ⚽ MIA-IRBI Football

[![Licença: MIT](https://img.shields.io/badge/Licença-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Status: Em Desenvolvimento](https://img.shields.io/badge/Status-Em%20Desenvolvimento-orange)]()

**Modelo preditivo para títulos da Copa do Mundo baseado em maturação coletiva (τ) e horizontalidade tática.**

> Em vez de talento bruto ou PIB, o MIA-IRBI mostra que **sistemas que amadurecem juntos e distribuem responsabilidade** são os verdadeiros favoritos.

---

## 📊 Resultados-chave

- **Acurácia retrospectiva (1998–2022):** 89,3%  
- **AUC (Área sob a curva ROC):** 0,94  
- **Variável mais importante:** `τ` (tempo de maturação coletiva) – p = 0,003  
- **Projeção para 2026:**  
  🇫🇷 França 29% | 🇪🇸 Espanha 21% | 🇯🇵 Japão 15% | 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra 11% | 🇧🇷 Brasil 2,8%

---

## 🧠 Metodologia

O modelo MIA-IRBI utiliza **quatro variáveis meso-analíticas**:

- **τ (tempo de maturação coletiva)** – anos de convivência do núcleo + estabilidade do técnico.
- **Simetria** – distribuição de responsabilidades (gols, assistências, desarmes). Quanto maior, menor a dependência de estrelas.
- **ρ_r (densidade relacional)** – coesão em passes e ocupação de espaço.
- **IRBI** – capacidade de reorganização sob pressão (viradas, substituições eficazes).

O modelo foi treinado com dados de **28 semifinalistas das Copas de 1998 a 2022**, utilizando regressão logística regularizada e validação cruzada *leave‑one‑cup‑out*.

---

## 📦 Instalação

```bash
git clone https://github.com/marcelobarbosa-ifalolu/MIA-IRBI-Football.git
cd MIA-IRBI-Football
pip install -r requirements.txt
