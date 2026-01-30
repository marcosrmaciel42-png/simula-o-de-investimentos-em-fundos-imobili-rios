# 📊 Simulação de Investimentos em Fundos Imobiliários (FIIs)

Este repositório contém uma planilha eletrônica desenvolvida para simular o crescimento patrimonial e a geração de renda passiva por meio de investimentos em Fundos de Investimento Imobiliário (FIIs), considerando variáveis financeiras reais como inflação e rendimento nominal.

O objetivo principal é fornecer uma ferramenta de planejamento financeiro que auxilie o investidor a visualizar o caminho para a independência financeira com base em **depósitos mensais** e alocações estratégicas.

---

## ✨ Funcionalidades Principais

A planilha está estruturada em três abas principais, cada uma com um propósito específico:

1. **Painel de Planejamento Financeiro:**
    * Apresenta de forma visual e resumida os principais indicadores de longo prazo.
    * Exibe o Patrimônio Real e a Renda Mensal Real ajustada ao longo de 30 anos.
    * Cálculo do Rendimento Real Mensal (já descontada a inflação).

2. **Calculadora Financeira:**
    * Permite a inserção de Variáveis de Entrada personalizadas, como salário mensal, percentual de investimento sugerido, rendimento nominal e inflação estimada.
    * Cálculo do Poder de Compra Real do patrimônio acumulado e dos dividendos mensais.
    * Apresenta a projeção de resultados em diferentes cenários de tempo (2, 5, 10, 20 e 30 anos).

3. **Estratégica:**
    * Definir uma distribuição percentual ideal dos **investimentos** entre as diferentes modalidades de FIIs, de acordo com o Perfil de Investidor selecionado (Conservador, Moderado ou Agressivo).

---

## 🧠 Lógica de Cálculo (Memória de Cálculo)

Para que o usuário compreenda como os dados são processados, a planilha utiliza os seguintes conceitos comerciais:

### 1. Taxa Real de Juros
Não basta subtrair a inflação do rendimento. Para encontrar o ganho real de poder de compra, utilizamos a **Equação de Fisher**:

$$i_{real} = \frac{1 + i_{nominal}}{1 + i_{inflação}} - 1$$

### 2. Acúmulo de Patrimônio (Juros Compostos)
A projeção de crescimento utiliza a fórmula de **Valor Futuro ($FV$)** de uma série de depósitos mensais:

$$FV = PMT \times \frac{(1 + i)^n - 1}{i}$$

*Onde: $PMT$ é o valor investido mensalmente, $i$ é a taxa de juros mensal e $n$ é o número de meses.*

### 3. Poder de Compra (Valor Presente)
Para ajustar os valores milionários do futuro à realidade atual (deflacionar), aplicamos:

$$VP = \frac{VF}{(1 + i_{inflação})^n}$$

*Isso permite saber quanto o patrimônio acumulado em 30 anos valeria com os preços de hoje.*

---

## 🛠️ Tipos de FIIs e Perfis de Investidor

A simulação utiliza uma classificação comum de FIIs e perfis de risco para a alocação:

| Tipo de FII | Descrição |
| :--- | :--- |
| **PAPEL** | Fundos que investem em títulos de dívida imobiliária (CRI, LCI, etc.). |
| **TIJOLO** | Fundos que investem em imóveis financeiros (lajes corporativas, shoppings, galpões logísticos). |
| **HÍBRIDOS** | Fundos que combinaram investimentos em títulos e imóveis financeiros. |
| **FOFs** | Fundos de Fundos, que investem em cotas de outros FIIs. |
| **DESENVOLVIMENTO** | Fundos focados na construção e venda de empreendimentos imobiliários. |
| **HOTELÁRIAS** | Fundos com foco em ativos do setor hoteleiro. |

A alocação percentual é ajustada automaticamente ao selecionar um dos seguintes perfis:

* **Conservador:** Maior foco em segurança e menor volatilidade.
* **Moderado:** Busca equilíbrio entre risco e retorno.
* **Agressivo:** Maior tolerância ao risco em busca de retornos mais elevados.

---

## 🚀 Como Utilizar

Para começar a simular seus investimentos, siga os passos abaixo:

1. **Download:** [[Clique aqui para baixar a Planilha de Simulação](https://github.com/marcosrmaciel42-png/simula-o-de-investimentos-em-fundos-imobili-rios/raw/refs/heads/main/Simula%C3%A7%C3%A3o%20de%20investimentos%20em%20fundos%20imobili%C3%A1rios..xlsx)]
2. **Ajuste as Variáveis:** Vá para a aba **Calculadora Financeira** e preencha seus dados nas Variáveis de Entrada (Salário, Investimento, Taxas).
3. **Selecione o Perfil:** Na mesma aba, escolha o seu Perfil de Investidor (Conservador, Moderado ou Agressivo).
4. **Visualize:** Volte ao **Dashboard** para ver os gráficos e indicadores atualizados com suas projeções personalizadas.

---

## ⚠️ Aviso Legal

Esta planilha é uma ferramenta de simulação e não constitui uma recomendação de investimento. Os resultados são baseados em previsões e estimativas que não podem se concretizar no futuro. O investimento em Fundos Imobiliários envolve riscos, e o desempenho passado não é garantia de resultados futuros. Consulte sempre um certificado profissional de investimentos antes de tomar qualquer decisão financeira.
