# 🎯 Desafio: Desenvolvimento de Componente Card Customizável

Esse desafio lhe fornecerá conhecimentos analíticos e desenvolverá suas habilidades de programação e raciocínio 
Esse desafio lhe ajudará a desenvolver suas habilidades para o mercado de trabalho lhe trazendo uma visão dos desafios diários do mercado de trabalho 

## 📋 Objetivo

Desenvolver um componente `Card` altamente customizável e reutilizável que possa ser utilizado em diferentes contextos da aplicação. O componente deve seguir os princípios de design system, ser responsivo e oferecer máxima flexibilidade de customização.
Use qualquer lingue

## 🎨 Requisitos Funcionais

### 1. **Estrutura do Card**

O componente deve suportar a seguinte estrutura:
- **Ícone/Avatar à esquerda ou direita** (opcional)
- **Título** (obrigatório)
- **Descrição** (opcional)
- **Ícone/Avatar à direita** (opcional)

### 2. **Customização de Cores Individuais**

O componente deve permitir customização individual de cores para:
- ✅ **Título**: Cor customizável via prop
- ✅ **Descrição**: Cor customizável via prop
- ✅ **Ícones** (esquerda e direita): Cor customizável via prop
- ✅ **Cor de fundo do card**: Customizável via prop

### 3. **Escala de Tamanhos**

Implementar uma escala de tamanhos responsiva com as seguintes opções:
- `xsm` - Extra pequeno
- `sm` - Pequeno
- `md` - Médio (padrão)
- `lg` - Grande
- `xl` - Extra grande
- `xxl` - Extra extra grande

Cada tamanho deve ajustar:
- Altura mínima do card
- Padding interno
- Tamanho da fonte do título
- Tamanho da fonte da descrição
- Tamanho dos ícones/avatar

### 4. **Responsividade**

O componente deve ser totalmente responsivo:
- Adaptar-se a diferentes tamanhos de tela (mobile, tablet, desktop)
- Ajustar espaçamentos e tamanhos conforme o viewport
- Manter legibilidade em todos os dispositivos
- Utilizar breakpoints apropriados

### 5. **Variantes de Estilo**

Implementar diferentes variantes de estilo:

#### 5.1. **Com/Sem Bordas**
- `bordered` - Card com borda visível
- `borderless` - Card sem borda

#### 5.2. **Com/Sem Fundo**
- `filled` - Card com cor de fundo
- `transparent` - Card sem fundo (transparente)
- `outlined` - Card apenas com borda, sem fundo

### 6. **Customização de Cor de Fundo**

Permitir customização da cor de fundo do card através de:
- Prop específica para cor de fundo
- Suporte a cores do design system
- Suporte a cores customizadas (hex, rgb, etc.)

## 💡 Dica de Desenvolvimento

> **Este desafio testa sua capacidade de raciocínio e atenção aos detalhes.**
> 
> Ao desenvolver o componente, considere todos os aspectos de customização visual. Pense em como cada elemento pode ser personalizado de forma independente e como diferentes combinações de propriedades podem interagir entre si.
> 
> **Lembre-se:** Um componente bem pensado considera não apenas os casos de uso mais comuns, mas também os cenários edge e as combinações menos óbvias de propriedades. Teste todos os cenários possíveis para garantir que sua solução seja robusta e completa.

## 📐 Especificações Técnicas

## ✅ Critérios de Aceitação

1. ✅ Componente renderiza corretamente com todos os elementos opcionais
2. ✅ Cores individuais funcionam independentemente (título, descrição, ícones)
3. ✅ Todos os tamanhos são implementados e responsivos
4. ✅ Variantes de estilo funcionam corretamente
5. ✅ Customização de cor de fundo funciona
6. ✅ Tests unitarios
7. ✅ Componente é responsivo em diferentes dispositivos
8. ✅ Componente aceita ícones e avatares
9. ✅ Componente é acessível (testID, aria-labels quando necessário)
10. ✅ Código está bem estruturado e documentado

## 🧪 Casos de Teste Sugeridos

1. Renderizar card apenas com título
2. Renderizar card com título e descrição
3. Renderizar card com ícone à esquerda
4. Renderizar card com ícone à direita
5. Renderizar card com avatar à esquerda
6. Testar todos os tamanhos (xsm a xxl)
7. Testar todas as variantes (filled, transparent, outlined)
8. Testar com e sem borda
9. Testar customização de cores
10. Testar customização individual de todas as cores
11. Testar responsividade em diferentes viewports
12. Testar estado disabled
13. Testar interatividade (onPress)

## 📝 Notas Adicionais

- Utilize TypeScript para type safety
- Siga os padrões de código do projeto
- Documente o componente adequadamente
- Considere performance e otimizações
- Mantenha o código limpo e reutilizável

## 🎁 Bônus (Opcional)

- Adicionar animações de hover/press
- Suporte a loading state
- Suporte a estado de erro
- Suporte a múltiplos layouts (horizontal, vertical, split)

---

## 📦 Como Entregar o Desafio

### Requisitos de Entrega

1. **Linguagem e Tecnologia**
   - Você pode utilizar qualquer linguagem de programação e framework de sua preferência
   - Exemplos: React, Vue, Angular, Svelte, HTML/CSS/JavaScript puro, etc.

2. **Formato de Entrega**
   - Desenvolva um **site/aplicação web** que demonstre o componente Card funcionando
   - O site deve estar acessível e funcional 

3. **Demonstração dos Modelos**
   - O site deve conter uma **galeria de exemplos** mostrando todos os modelos e variações do Card
   - Demonstre pelo menos:
     - Todos os tamanhos (xsm, sm, md, lg, xl, xxl)
     - Todas as variantes (filled, transparent, outlined)
     - Diferentes combinações de ícones/avatar
     - Exemplos com customização de cores individuais
     - Exemplos responsivos

4. **Documentação**
   - Inclua um README explicando como executar o projeto
   - Documente as props e como utilizar o componente

---

**Boa sorte no desenvolvimento! 🚀**

