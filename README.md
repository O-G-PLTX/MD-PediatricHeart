# MD-PediatricHeart

`MD-PediatricHeart` é um conjunto de dados clínicos voltado para o estudo, análise e predição de **condições cardíacas em crianças e adolescentes**, com idade entre **0 e 19 anos**. Os dados foram coletados no **Real Hospital Português (RHP)**, em Recife–PE, e anonimizados com aprovação do Comitê de Ética do RHP e da Universidade do Porto, Portugal.

Este repositório foi criado para centralizar a documentação, exploração, preparação e modelagem dos dados, seguindo as etapas do processo de **Knowledge Discovery in Databases (KDD)**.

---

## 📊 Sobre os dados

- **Total de registros (pacientes):** 1417  
- **Número de atributos:** 21  
- **Idade dos pacientes:** de 0 a 19 anos  
- **Variável-alvo:** `NORMAL X ANORMAL` (indica se há patologia cardíaca)

---

## 🧾 Dicionário de Dados

| Atributo             | Tipo        | Escala         | Descrição                                                                 |
|----------------------|-------------|----------------|---------------------------------------------------------------------------|
| `ID`                 | Categórico  | Nominal        | Identificador único do paciente (anonimizado)                            |
| `Peso`               | Numérico    | Razão          | Peso do paciente (kg)                                                    |
| `Altura`             | Numérico    | Razão          | Altura do paciente (cm)                                                  |
| `IMC`                | Numérico    | Razão          | Índice de Massa Corporal: peso / (altura em metros)²                     |
| `Atendimento`        | Temporal    | Data           | Data do atendimento médico                                               |
| `DN`                 | Temporal    | Data           | Data de nascimento do paciente                                           |
| `IDADE`              | Numérico    | Intervalar     | Idade em anos decimais, calculada com base nas datas                     |
| `Convenio`           | Categórico  | Nominal        | Tipo de convênio do paciente (ex: GS, SULA, SAME)                        |
| `PULSOS`             | Categórico  | Ordinal        | Condição da pulsação (ex: Normais, Diminuídos, etc.)                     |
| `PA SISTOLICA`       | Numérico    | Intervalar     | Pressão Arterial Sistólica (mmHg)                                        |
| `PA DIASTOLICA`      | Numérico    | Intervalar     | Pressão Arterial Diastólica (mmHg)                                       |
| `PPA`                | Numérico / Texto | Razão / Texto | Razão entre PAS e PAD; alguns casos estão como "Não Calculado"        |
| `NORMAL X ANORMAL`   | Categórico  | Binário        | Indica se o paciente tem (Anormal) ou não tem (Normal) patologia cardíaca |
| `B2`                 | Categórico  | Nominal        | Tipo do segundo som cardíaco (bulha B2)                                  |
| `SOPRO`              | Categórico  | Nominal        | Presença ou tipo de sopro cardíaco identificado                          |
| `FC`                 | Numérico    | Intervalar     | Frequência cardíaca (batimentos por minuto)                              |
| `HDA 1`              | Categórico  | Nominal        | Queixa principal ou histórico da doença atual                            |
| `HDA2`               | Categórico  | Nominal        | Queixa secundária (quando presente)                                      |
| `SEXO`               | Categórico  | Nominal        | Sexo biológico do paciente (`M` ou `F`)                                  |
| `MOTIVO1`            | Categórico  | Nominal        | Principal motivo de encaminhamento para a cardiologia                    |
| `MOTIVO2`            | Categórico  | Nominal        | Motivo secundário de encaminhamento (se houver)                          |

---

## 📘 Sobre esta atividade

Este repositório faz parte de uma **atividade prática da disciplina de Mineração de Dados**, com foco em aplicar conceitos de KDD em dados reais e sensíveis da área da saúde.

### 👥 Integrantes do grupo:
**Wagner Victor Alves de Menezes**  
**Raphael Alves**  
**Victor Gabriel**

---

