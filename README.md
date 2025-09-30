
# WCST-64 - Wisconsin Card Sorting Test

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-green.svg)](https://github.com)
[![Responsive](https://img.shields.io/badge/responsive-yes-brightgreen.svg)](https://github.com)

## 📋 Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Características](#características)
- [Fundamentos Científicos](#fundamentos-científicos)
- [Instalação](#instalação)
- [Uso](#uso)
- [Parâmetros e Métricas](#parâmetros-e-métricas)
- [Exportação de Dados](#exportação-de-dados)
- [Interpretação dos Resultados](#interpretação-dos-resultados)
- [Compatibilidade](#compatibilidade)
- [Referências](#referências)
- [Licença](#licença)
- [Contato](#contato)

## 🧠 Sobre o Projeto

Implementação moderna e responsiva do **Wisconsin Card Sorting Test (WCST-64)**, um dos testes neuropsicológicos mais utilizados para avaliar funções executivas e flexibilidade cognitiva.

Esta versão web foi desenvolvida seguindo as melhores práticas experimentais documentadas na literatura científica, sendo totalmente autoaplicável em dispositivos móveis, tablets e computadores.

### Histórico

O WCST foi originalmente desenvolvido por **Esta Berg** e **David Grant** em 1948 na University of Wisconsin, para medir raciocínio abstrato e flexibilidade no pensamento. Posteriormente, **Brenda Milner** (1963) demonstrou sua sensibilidade para detectar disfunções do córtex pré-frontal dorsolateral.

## ✨ Características

### Design e Usabilidade
- ✅ **100% Responsivo** - Mobile-first design com adaptação automática
- ✅ **Touch-Optimized** - Áreas de toque ≥44px conforme guidelines de acessibilidade
- ✅ **Sem Instalação** - Execução direta no navegador (HTML5)
- ✅ **Offline-Ready** - Funciona sem conexão após primeiro carregamento
- ✅ **Multiplataforma** - iOS, Android, Windows, macOS, Linux

### Funcionalidades Técnicas
- 🎯 **Paradigma Experimental Validado** - Baseado em Heaton et al. (1993)
- 📊 **Análise Automática** - Cálculo de erros perseverativos e não-perseverativos
- 💾 **Múltiplos Formatos de Exportação** - PDF, CSV, JSON
- ⏱️ **Registro Temporal** - Timestamp de cada tentativa
- 🔒 **Privacidade** - Dados processados localmente no navegador

### Características do Teste
- **64 tentativas** (versão reduzida do WCST original de 128 cartas)
- **3 dimensões de classificação**: Cor, Forma, Número
- **4 cartas estímulo fixas**
- **Mudança automática de regra** após 10 acertos consecutivos
- **Feedback imediato** após cada resposta

## 🔬 Fundamentos Científicos

### O Que o WCST Avalia

O teste mensura componentes das **funções executivas**, especificamente:

1. **Raciocínio Abstrato** - Capacidade de formar conceitos
2. **Set-Shifting** - Flexibilidade para mudar estratégias
3. **Feedback Processing** - Uso eficiente de informação ambiental
4. **Working Memory** - Manutenção de regras ativas
5. **Inibição de Resposta** - Controle de perseveração

### Sensibilidade Clínica

O WCST tem sido usado para avaliar pacientes com:

- Lesões do córtex pré-frontal
- Esquizofrenia
- Transtorno do Espectro Autista (TEA)
- TDAH (Transtorno de Déficit de Atenção/Hiperatividade)
- Doenças neurodegenerativas (Parkinson, Alzheimer)
- AVC (Acidente Vascular Cerebral)
- Traumatismo cranioencefálico

### Paradigma Experimental Implementado

#### Estrutura das Cartas

**4 Cartas Estímulo (fixas):**
1. 1 triângulo vermelho
2. 2 estrelas verdes
3. 3 cruzes azuis
4. 4 círculos amarelos

**Carta de Resposta (variável):**
- Combinação aleatória de cor, forma e número
- Pode corresponder a múltiplas dimensões (ambiguidade intencional)

#### Regras de Classificação

O participante deve descobrir qual dimensão está ativa:
- **Cor**: vermelho, verde, azul, amarelo
- **Forma**: círculo, estrela, triângulo, cruz
- **Número**: 1, 2, 3, 4

#### Critério de Mudança

A regra muda automaticamente após **10 respostas corretas consecutivas**, sem aviso prévio ao participante.

#### Classificação de Erros

**Erro Perseverativo:**
- Ocorre quando o participante continua aplicando a regra anterior
- Indica dificuldade em inibir estratégias previamente reforçadas

**Erro Não-Perseverativo:**
- Qualquer outro tipo de erro
- Pode indicar falha na formação de conceito ou erro aleatório

## 🚀 Instalação

### Opção 1: Uso Direto (Recomendado)

1. Baixe o arquivo `wcst-64.html`
2. Abra em qualquer navegador moderno
3. Pronto para usar!

### Opção 2: Servidor Local

```bash
# Com Python 3
python -m http.server 8000

# Com Node.js
npx http-server

# Acesse: http://localhost:8000
```

### Opção 3: Hospedagem Web

Faça upload do arquivo HTML para qualquer serviço de hospedagem:
- GitHub Pages
- Netlify
- Vercel
- Firebase Hosting

## 📖 Uso

### Fluxo do Teste

1. **Tela Inicial** - Apresentação e contextualização
2. **Instruções** - Explicação detalhada das regras
3. **Teste** - 64 tentativas com feedback imediato
4. **Resultados** - Análise automática e interpretação

### Instruções para o Participante

```
"Você verá 4 cartas de referência na parte superior e 1 carta 
de resposta abaixo. Seu objetivo é descobrir a regra para 
combinar a carta de resposta com uma das cartas de referência.

Você pode combinar por COR, FORMA ou NÚMERO.

Clique na carta que você acha que combina. Você receberá 
feedback se está correto ou incorreto.

A regra pode mudar sem aviso durante o teste. Use o feedback 
para descobrir quando isso acontecer."
```

### Recomendações de Aplicação

- **Ambiente**: Silencioso, sem distrações
- **Tempo**: 10-15 minutos (sem limite rígido)
- **Idade**: A partir de 6.5 anos
- **Instruções**: Ler em voz alta ou permitir leitura autônoma
- **Prática**: Não há tentativas de treino (aprendizagem faz parte do teste)

## 📊 Parâmetros e Métricas

### Métricas Principais

| Métrica | Descrição | Interpretação |
|---------|-----------|---------------|
| **Total de Tentativas** | Número fixo de cartas apresentadas | 64 (padrão) |
| **Erros Totais** | Soma de todos os erros | Menor = melhor |
| **Taxa de Erro (%)** | (Erros / 64) × 100 | < 25% = normal |
| **Erros Perseverativos** | Erros usando regra anterior | Indicador de rigidez cognitiva |
| **Erros Não-Perseverativos** | Outros erros | Indicador de formação de conceito |
| **% Perseverativo** | (Pers / Total Erros) × 100 | > 50% = alta perseveração |
| **Categorias Completadas** | Séries de 10 acertos | 5-6 = excelente |
| **Tempo Total** | Duração do teste | Variável (sem limite) |

### Dados por Tentativa (Trial-Level)

Cada tentativa registra:
- Número da tentativa (1-64)
- Regra ativa (cor/forma/número)
- Carta de resposta (cor, forma, número)
- Carta selecionada (índice 0-3)
- Resultado (correto/incorreto)
- Tipo de erro (perseverativo/não-perseverativo/N/A)
- Timestamp (ISO 8601)
- Sequência de acertos consecutivos

## 💾 Exportação de Dados

### Formato PDF

Relatório formatado para impressão contendo:
- Cabeçalho com data/hora
- Resumo executivo das métricas
- Interpretação qualitativa
- Ideal para: laudos clínicos, relatórios

**Arquivo gerado**: `wcst-64-resultado.pdf`

### Formato CSV

Dados tabulares compatíveis com análise estatística:

```csv
Tentativa,Regra,Cor_Resposta,Forma_Resposta,Numero_Resposta,Carta_Selecionada,Correto,Tipo_Erro,Timestamp
1,color,red,star,3,0,true,N/A,2025-09-30T10:23:45.123Z
2,color,blue,circle,2,1,false,non-perseverative,2025-09-30T10:23:48.456Z
...
```

**Compatível com:**
- SPSS, R, Python (pandas)
- Excel, Google Sheets
- Tableau, Power BI

**Arquivo gerado**: `wcst-64-dados.csv`

### Formato JSON

Estrutura completa hierárquica:

```json
{
  "testInfo": {
    "name": "WCST-64",
    "version": "1.0",
    "date": "2025-09-30T10:23:45.123Z"
  },
  "summary": {
    "totalTrials": 64,
    "totalErrors": 18,
    "perseverativeErrors": 9,
    "nonPerseverativeErrors": 9,
    "completedCategories": 4,
    "durationSeconds": 720
  },
  "trials": [...]
}
```

**Ideal para:**
- Processamento programático
- APIs e integrações
- Análises customizadas

**Arquivo gerado**: `wcst-64-completo.json`

## 📈 Interpretação dos Resultados

### Classificação de Desempenho

#### Categorias Completadas

| Categorias | Classificação | Interpretação |
|------------|---------------|---------------|
| 5-6 | Excelente | Flexibilidade cognitiva superior |
| 3-4 | Bom | Desempenho adequado |
| 1-2 | Abaixo da Média | Dificuldade moderada |
| 0 | Deficitário | Rigidez cognitiva significativa |

#### Erros Perseverativos

| % Perseverativo | Interpretação |
|-----------------|---------------|
| < 30% | Normal |
| 30-50% | Leve tendência à perseveração |
| 50-70% | Perseveração moderada |
| > 70% | Perseveração severa |

### Padrões Clínicos Comuns

**Alta Perseveração + Poucas Categorias:**
- Sugere disfunção do córtex pré-frontal dorsolateral
- Comum em lesões frontais, esquizofrenia

**Muitos Erros Não-Perseverativos:**
- Dificuldade na formação inicial de conceitos
- Pode indicar déficit de atenção ou working memory

**Tempo Prolongado:**
- Pode indicar indecisão, ansiedade ou lentidão processual
- Considerar fatores emocionais

### ⚠️ Limitações e Considerações

1. **Não é diagnóstico**: O WCST é uma ferramenta de triagem, não substitui avaliação completa
2. **Influência de variáveis**: Idade, escolaridade, QI afetam o desempenho
3. **Especificidade**: Teste pode ser alterado por danos em várias regiões cerebrais
4. **Contexto**: Sempre interpretar junto com história clínica e outros testes

## 🖥️ Compatibilidade

### Navegadores Suportados

| Navegador | Versão Mínima | Status |
|-----------|---------------|--------|
| Chrome | 90+ | ✅ Testado |
| Firefox | 88+ | ✅ Testado |
| Safari | 14+ | ✅ Testado |
| Edge | 90+ | ✅ Testado |
| Opera | 76+ | ✅ Compatível |
| Samsung Internet | 14+ | ✅ Compatível |

### Dispositivos

- 📱 **Smartphones**: iOS 12+, Android 8+
- 📱 **Tablets**: iPad, Android tablets
- 💻 **Desktop**: Windows 10+, macOS 10.14+, Linux
- 🖥️ **Resoluções**: 320px - 4K

### Requisitos Técnicos

- **JavaScript**: Habilitado (essencial)
- **Cookies**: Não necessário
- **Conexão**: Apenas no primeiro acesso
- **Armazenamento**: ~500KB

## 📚 Referências

### Artigos Fundamentais

1. **Berg, E. A. (1948)**. A simple objective technique for measuring flexibility in thinking. *Journal of General Psychology*, 39, 15-22.

2. **Grant, D. A., & Berg, E. A. (1948)**. A behavioral analysis of degree of reinforcement and ease of shifting to new responses in a Weigl-type card-sorting problem. *Journal of Experimental Psychology*, 38, 404-411.

3. **Milner, B. (1963)**. Effects of different brain lesions on card sorting. *Archives of Neurology*, 9, 90-100.

4. **Heaton, R. K., Chelune, G. J., Talley, J. L., Kay, G. G., & Curtiss, G. (1993)**. *Wisconsin Card Sorting Test Manual: Revised and Expanded*. Psychological Assessment Resources.

5. **Nelson, H. E. (1976)**. A modified card sorting test sensitive to frontal lobe defects. *Cortex*, 12, 313-324.

### Revisões e Meta-Análises

6. **Nyhus, E., & Barceló, F. (2009)**. The Wisconsin Card Sorting Test and the cognitive assessment of prefrontal executive functions: A critical update. *Brain and Cognition*, 71(3), 437-451.

7. **Lange, F., Seer, C., & Kopp, B. (2017)**. Cognitive flexibility in neurological disease: Cognitive components and event-related potentials. *Neuroscience & Biobehavioral Reviews*, 83, 496-507.

### Normas e Padronização

8. **Schretlen, D. J. (2010)**. *Modified Wisconsin Card Sorting Test (M-WCST): Professional Manual*. Psychological Assessment Resources.

## 📄 Licença

Este projeto está licenciado sob a **MIT License** - veja o arquivo [LICENSE](LICENSE) para detalhes.

```
MIT License

Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

### Uso Clínico

Para uso clínico, recomenda-se:
- Registro no conselho profissional apropriado
- Supervisão adequada para aplicação e interpretação
- Consentimento informado dos participantes
- Conformidade com regulamentações locais (CFP, APA, etc.)

## 🤝 Contribuições

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

### Áreas para Contribuição

- [ ] Tradução para outros idiomas
- [ ] Integração com REDCap/LimeSurvey
- [ ] Versão com 128 cartas (WCST completo)
- [ ] Análise de curva de aprendizagem
- [ ] Visualizações gráficas interativas
- [ ] Modo para pesquisadores (customizações)


---

## ⚕️ Aviso Ético

Este software é fornecido apenas para fins educacionais e de pesquisa. Não substitui avaliação neuropsicológica profissional. Profissionais devem ter treinamento adequado para administração e interpretação do WCST conforme normas éticas e regulamentações locais.

**Desenvolvido com base em literatura científica e boas práticas em neuropsicologia computacional.**

---

**Versão**: 1.0.0  
**Última Atualização**: Setembro 2025  
**Status**: Produção
