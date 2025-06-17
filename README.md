# xbox-subscriptions-dashboard-excel - Excel with AI Project
 
Visualização interativa do painel de assinaturas Xbox

## 🎯 Objetivo
Dashboard desenvolvido para análise estratégica das assinaturas Xbox, permitindo:
- Monitoramento em tempo real dos tipos de assinatura
- Comparação entre EA Play e Minecraft Season Pass
- Tomada de decisão baseada em tendências de consumo

## 📦 Dados Utilizados

- **Fonte**: Dados anônimos de assinaturas Xbox (2024)
- **Estrutura**:
  - Subscription Type (Annual/Monthly/Quarterly)
  - EA Play Season Pass subscriptions
  - Minecraft Season Pass subscriptions
  - Período de coleta (cabeçalho informativo)

## 🛠️ Funcionalidades Principais
### *1. Personalização Dinâmica*
- Mensagem de boas-vindas com nome do usuário logado  
  ="Bem vindo (a), " & USERNAME & "!"

### *2. Filtros Interativos*
- *Subscription Type* (botões de seleção):
  - Annual | Monthly | Quarterly
  - Atualiza todos os componentes do dashboard

### *3. Cards de Métricas*
| Card | Fórmula Exemplo |
|------|-----------------|
| TOTAL EA PLAY | =SUMIFS(Tabela[EA Play], Tabela[Type], "Annual") |
| TOTAL MINECRAFT | =SUMIFS(Tabela[Minecraft], Tabela[Type], "Annual") |

### *4. Visualização Gráfica*
- Gráfico combinado (colunas + linha) mostrando:
  - Volume por tipo de assinatura
  - Proporção EA Play vs Minecraft

## 📥 Como Utilizar
1. *Abrir o arquivo* dashboard_de_vendas_do_xbox.xlsx (versão 365 ou 2021)
2. *Atualizar dados* (se necessário):
   - Acesse Data → Refresh All
3. *Interagir*:
   - Clique nos botões de Subscription Type
   - Observe a atualização automática dos cards e gráficos

## ⚙️ Tecnologias Aplicadas
- *Excel Avançado*:
  - Tabelas dinâmicas com FILTER()
  - Formatação condicional 


## 📸 Screenshots
![Filtros](/screenshots/filters.png)  
Seleção de Subscription Type

![Gráficos](/screenshots/charts.png)  
Visualização comparativa
