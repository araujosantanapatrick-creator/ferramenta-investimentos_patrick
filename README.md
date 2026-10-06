# Ferramenta de Investimentos

Planilha em Excel para simulação de planejamento de investimentos em FIIs.

## O que a ferramenta responde

A ferramenta responde a cinco perguntas:

1. **Quanto investir por mês?**  
   O valor aparece em **Configurações > Aporte mensal**. O aporte sugerido inicialmente corresponde a 30% do salário.

2. **Por quantos anos investir?**  
   O prazo é informado em **Anos de investimento**. A planilha também apresenta projeções para 2, 5, 10, 20 e 30 anos.

3. **Qual a taxa de rendimento mensal?**  
   O usuário informa a **Taxa de rendimento mensal**. A simulação utiliza inicialmente 0,8% ao mês.

4. **Quanto de patrimônio será acumulado?**  
   O resultado aparece na área **Respostas > Patrimônio acumulado**.

5. **Quanto poderá receber de dividendos por mês?**  
   O resultado aparece na área **Respostas > Dividendos mensais**.

## VF e PROCV

A função **VF (Valor Futuro)** é utilizada para calcular o patrimônio acumulado a partir da taxa de rendimento, quantidade de meses e aporte periódico.

A função **PROCV** é utilizada para buscar o percentual de distribuição correspondente à combinação entre o perfil escolhido e o tipo de FII.

Exemplo de chave utilizada:

`Moderado|Tijolo`

Quando o perfil é alterado, o PROCV busca os novos percentuais e a divisão do aporte é atualizada automaticamente.

## Intervalos nomeados

Foram utilizados intervalos nomeados para facilitar a leitura e manutenção das fórmulas:

- `salario`
- `aporte`
- `taxa_mensal`
- `anos`
- `perfil`
- `lista_perfis`
- `chave_perfil_fii`
- `percentuais_perfil_fii`

## Perfis e percentuais

### Conservador

- Tijolo: 30%
- Papel: 25%
- Híbrido: 20%
- FOF: 10%
- Desenvolvimento: 5%
- Agro: 10%

**Total: 100%**

### Moderado

- Tijolo: 25%
- Papel: 20%
- Híbrido: 20%
- FOF: 10%
- Desenvolvimento: 10%
- Agro: 15%

**Total: 100%**

### Arrojado

- Tijolo: 15%
- Papel: 15%
- Híbrido: 20%
- FOF: 10%
- Desenvolvimento: 20%
- Agro: 20%

**Total: 100%**

Os percentuais são uma distribuição-modelo criada para a simulação e não representam recomendação individual de investimento.

## Alterações em relação à ferramenta do Expert

A ferramenta foi simplificada e reorganizada para facilitar o uso.

Principais alterações:

- criação de uma área específica para as cinco respostas;
- separação entre configurações e resultados;
- seleção do perfil por lista;
- distribuição automática do aporte por tipo de FII;
- utilização de VF no cálculo do patrimônio;
- utilização de PROCV para buscar os percentuais;
- criação de intervalos nomeados;
- inclusão de projeções para diferentes prazos;
- criação de uma aba de apoio com os perfis e percentuais.

## Evidência de funcionamento

A mesma simulação foi realizada utilizando dois perfis diferentes.

### Perfil Moderado

![Perfil Moderado](perfil-moderado.png)

### Perfil Arrojado

![Perfil Arrojado](perfil-arrojado.png)

A troca do perfil altera automaticamente a divisão do aporte, mantendo cada perfil com distribuição total de 100%.

## Como usar

1. Informe o salário.
2. Confira ou altere o aporte mensal.
3. Informe a taxa de rendimento.
4. Escolha o prazo.
5. Selecione o perfil.
6. Confira os resultados e a divisão do aporte.

## Observação

Os valores utilizados na planilha publicada são exemplos para demonstração da ferramenta.
