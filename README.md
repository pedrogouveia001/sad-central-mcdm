# Nexus MCDM — Central Hub de Apoio à Decisão Multicritério

Este repositório é o núcleo central do **NEXUS MCDM**, um ecossistema integrado de Apoio à Decisão Multicritério (MCDM) desenvolvido com Flask e SQLAlchemy para auxiliar tomadores de decisão a estruturar, avaliar e resolver problemas complexos sob racionalidades compensatórias e não-compensatórias.

---

## 🎨 Identidade Visual e Branding
- **Nome Oficial:** Nexus MCDM
- **Cores Oficiais:** Roxo Real (`#8B5CF6`) e Verde Esmeralda (`#10B981`)
- **Conceito Visual:** Rede de nós interconectados formando a letra 'N' representando sinergia, conexões e integração de múltiplos decisores e métodos.
- **Copyright:** Direitos Reservados © 2026 NEXUS-MCDM. Todos os direitos reservados.

---

## 🌟 Recursos Principais

- **Suporte a 10 Solucionadores Multicritério:**
  - **Racionalidade Compensatória:**
    - **SMARTS:** Elicitação direta de pesos swing e normalização de intervalo.
    - **SMARTER:** Atribuição simplificada de pesos ordinais via centroides ROC.
    - **AHP (Analytic Hierarchy Process):** Matrizes de comparações par a par de Saaty e análise de consistência (CR).
    - **MACBETH:** Comparações qualitativas semânticas resolvidas por Programação Linear.
    - **BWM (Best Worst Method):** Otimização linear minimax baseada em comparações estruturadas.
    - **BWT (Best Worst Tradeoff):** Taxas de tradeoff inter-critério resolvidas por PL e bisseção intra-critério.
    - **TOPSIS:** Vetores de distância euclidiana às soluções ideal e anti-ideal.
    - **VIKOR:** Solução de compromisso ponderando utilidade de grupo e arrependimento.
  - **Racionalidade Não-Compensatória:**
    - **ELECTRE (TRI, I, IS, II, III, IV):** Relações de sobreclassificação baseadas em concordância, discordância e veto absoluto.
    - **PROMETHEE (I, II, III, IV, V, VI, TRI):** Fluxos de preferências líquidos e otimização inteira de portfólio de projetos (PROMETHEE V).
- **Importador Matriz TCC:** Permite importar planilhas Excel nos formatos `.xls`, `.xlsx` e `.csv` no layout da Matriz de Consequências do TCC (Linha 1: Critérios, Linha 2: Tipos, Linha 7: Níveis, Linha 9+: Consequências), com proteção contra valores `NaN` e `inf`.
- **Relatório em PDF com ReportLab:** Geração em tempo real de relatórios executivos de decisão completos e paginados, com tabelas dinâmicas e logotipo do método ativo.
- **Simulação de Monte Carlo:** Análise de robustez e estabilidade estatística do ranking sob perturbação estocástica dos dados.

---

## 📂 Estrutura do Projeto

```text
sad-central-mcdm/
├── app.py                # Servidor Flask e rotas controladoras
├── config.py             # Configurações do app e compartilhamento do banco SQLite
├── requirements.txt      # Dependências
├── models/               # Modelagem do banco de dados (SQLAlchemy)
├── modules/              # Engines matemáticas de cada resolvedor
├── services/             # Geração de PDFs e simulação de Monte Carlo
├── static/               # CSS customizado, JS e Logotipos da marca
└── templates/            # Telas HTML (assistente, matrizes e resultados)
```

---

## 🚀 Como Executar

### 1. Preparar Ambiente e Dependências
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1   # Windows
pip install -r requirements.txt
```

### 2. Rodar o Servidor
```powershell
python app.py
```
Acesse no navegador: `http://127.0.0.1:5000`
