# Nexus MCDM — Central Hub de Apoio à Decisão Multicritério

Este repositório é o núcleo central do **NEXUS MCDM**, um ecossistema integrado de Apoio à Decisão Multicritério (MCDM) desenvolvido com Flask e SQLAlchemy para auxiliar tomadores de decisão a estruturar, avaliar e resolver problemas complexos sob racionalidades compensatórias e não-compensatórias.

---

## 🎨 Identidade Visual e Branding
- **Nome Oficial:** Nexus MCDM
- **Cores Oficiais:** Roxo Real (`#8B5CF6`) e Verde Esmeralda (`#10B981`)
- **Conceito Visual:** Rede de nós interconectados formando a letra 'N' representando sinergia, conexões e integração de múltiplos decisores e métodos.
- **Copyright:** Direitos Reservados © 2026 NEXUS-MCDM. Todos os direitos reservados.

---

## 🏛️ Racionalidades e Métodos Suportados

O **NEXUS MCDM** unifica as duas grandes correntes de decisão multicritério:

### 1. Racionalidade Compensatória (Escola Americana)
Permite a compensação de desempenhos ruins em certos critérios por excelentes desempenhos em outros.
* **SMARTS / SMARTER**: Elicitação direta (Swing) e ordinal (Rank Order Centroid - ROC).
* **AHP (Analytic Hierarchy Process)**: Estrutura hierárquica e julgamento de matrizes de consistência par a par ($CR < 0.10$).
* **BWM (Best Worst Method)**: Otimização minimax linear com apenas $2n-3$ comparações.
* **BWT (Best Worst Tradeoff)**: Combinação da otimização BWM com taxas físicas de tradeoff inter-critério.
* **MACBETH**: Julgamentos qualitativos convertidos em escalas cardinais de utilidade através de Programação Linear.
* **TOPSIS**: Ordenação baseada na menor distância euclidiana da solução ideal e maior distância da anti-ideal.
* **VIKOR**: Solução de compromisso ponderando a utilidade de grupo ($S$) e o arrependimento individual ($R$).

### 2. Racionalidade Não-Compensatória (Escola Francesa / Outranking)
Impede a compensação ilimitada através de relações de sobreclassificação baseadas em concordância, discordância e limites estritos de veto.
* **ELECTRE (I, IS, II, III, IV, TRI)**: Relações de preferência nítidas e credibilidade de sobreclassificação ($\sigma$) usando pseudo-critérios.
* **PROMETHEE (I, II, III, IV, V, VI, TRI)**: Fluxos líquidos de preferência ($\Phi = \Phi^+ - \Phi^-$) e otimização inteira 0-1 (PROMETHEE V) para seleção de portfólios sob restrições físicas e financeiras.

---

## 🛠️ Detalhes do Desenvolvimento e Instalação

### Requisitos Mínimos
* Python 3.8 ou superior
* Bibliotecas listadas no `requirements.txt` (Flask, Pandas, NumPy, ReportLab, OpenPyXL, XLRD)

### Como rodar localmente
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python app.py
```
Acesse no navegador: `http://127.0.0.1:5000`

---

## 🛡️ Direitos Autorais
Direitos Reservados © 2026 NEXUS-MCDM. Todos os direitos reservados.
