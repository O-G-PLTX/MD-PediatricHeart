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

| Atributo             | Tipo         | Escala                | Descrição                                                                 |
|----------------------|--------------|------------------------|---------------------------------------------------------------------------|
| `ID`                 | Qualitativo  | Nominal                | Identificador único do paciente (anonimizado)                            |
| `Peso`               | Quantitativo | Razão                  | Peso do paciente (kg)                                                    |
| `Altura`             | Quantitativo | Razão                  | Altura do paciente (cm)                                                  |
| `IMC`                | Quantitativo | Razão                  | Índice de Massa Corporal: peso / (altura em metros)²                     |
| `Atendimento`        | Quantitativo | Intervalar             | Data do atendimento médico                                               |
| `DN`                 | Quantitativo | Intervalar             | Data de nascimento do paciente                                           |
| `IDADE`              | Quantitativo | Razão                  | Idade em anos decimais, calculada com base nas datas                     |
| `Convenio`           | Qualitativo  | Nominal                | Tipo de convênio do paciente (ex: GS, SULA, SAME)                        |
| `PULSOS`             | Qualitativo  | Ordinal                | Condição da pulsação (ex: Normais, Diminuídos, etc.)                     |
| `PA SISTOLICA`       | Quantitativo | Intervalar             | Pressão Arterial Sistólica (mmHg)                                        |
| `PA DIASTOLICA`      | Quantitativo | Intervalar             | Pressão Arterial Diastólica (mmHg)                                       |
| `PPA`                | Qualitativo* | Nominal* / Razão       | Razão entre PAS e PAD; alguns registros são texto ("Não Calculado")      |
| `NORMAL X ANORMAL`   | Qualitativo  | Nominal                | Indica se há (Anormal) ou não há (Normal) patologia cardíaca             |
| `B2`                 | Qualitativo  | Nominal                | Tipo do segundo som cardíaco (bulha B2)                                  |
| `SOPRO`              | Qualitativo  | Nominal                | Presença ou tipo de sopro cardíaco identificado                          |
| `FC`                 | Quantitativo | Intervalar             | Frequência cardíaca (batimentos por minuto)                              |
| `HDA 1`              | Qualitativo  | Nominal                | Queixa principal ou histórico da doença atual                            |
| `HDA2`               | Qualitativo  | Nominal                | Queixa secundária (quando presente)                                      |
| `SEXO`               | Qualitativo  | Nominal                | Sexo biológico do paciente (`M` ou `F`)                                  |
| `MOTIVO1`            | Qualitativo  | Nominal                | Principal motivo de encaminhamento para a cardiologia                    |
| `MOTIVO2`            | Qualitativo  | Nominal                | Motivo secundário de encaminhamento (se houver)                          |

> ℹ️ *Nota sobre `PPA`: como contém tanto valores numéricos quanto texto (“Não Calculado”), seu tipo é misto. Pode ser tratado como **Qualitativo Nominal** nos registros não numéricos e **Quantitativo Razão** quando houver valor válido.


---

## 📘 Sobre esta atividade

Este repositório faz parte de uma **atividade prática da disciplina de Mineração de Dados**, com foco em aplicar conceitos de KDD em dados reais e sensíveis da área da saúde.

### 👥 Integrantes do grupo:
**Wagner Victor Alves de Menezes**  
**Raphael Alves**  
**Victor Gabriel**

---

