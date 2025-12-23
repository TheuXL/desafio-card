# 🎯 Desafio: Desenvolvimento de Componente Card Customizável

## 📋 Objetivo

Desenvolver um componente `Card` altamente customizável e reutilizável que possa ser utilizado em diferentes contextos da aplicação. O componente deve seguir os princípios de design system, ser responsivo e oferecer máxima flexibilidade de customização.

## 🎨 Requisitos Funcionais

### 1. **Estrutura do Card**

O componente deve suportar a seguinte estrutura:
- **Ícone/Avatar à esquerda ou direita** (opcional)
- **Título** (obrigatório)
- **Descrição** (opcional)
- **Ícone à direita** (opcional)

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

## ⚠️ ATENÇÃO ESPECIAL: Customização de Cor da Borda

> **🔴 IMPORTANTE: Este é um requisito crítico que muitos desenvolvedores esquecem!**
> 
> O componente **DEVE** suportar customização da cor da borda de forma independente da cor de fundo e das outras propriedades.
> 
> **Pense bem:** Como você vai implementar isso? 
> - A cor da borda deve ser configurável via prop
> - Deve funcionar em conjunto com as variantes (bordered/borderless)
> - Deve respeitar o design system mas também permitir cores customizadas
> - Considere casos edge como: borda colorida com fundo transparente, borda customizada com variante outlined, etc.
> 
> **Dica:** Não esqueça de testar todos os cenários possíveis de combinação entre cor de borda, cor de fundo e variantes!

## 📐 Especificações Técnicas

### Props do Componente

```typescript
interface CardComponentProps {
  // Conteúdo
  title: string;
  description?: string;
  leftIcon?: React.ReactNode | string; // Ícone ou avatar
  rightIcon?: React.ReactNode | string;
  
  // Cores individuais
  titleColor?: string;
  descriptionColor?: string;
  leftIconColor?: string;
  rightIconColor?: string;
  backgroundColor?: string;
  borderColor?: string; // ⚠️ NÃO ESQUECER!
  
  // Tamanhos
  size?: 'xsm' | 'sm' | 'md' | 'lg' | 'xl' | 'xxl';
  
  // Variantes
  variant?: 'filled' | 'transparent' | 'outlined';
  borderVariant?: 'bordered' | 'borderless';
  
  // Interatividade
  onPress?: () => void;
  disabled?: boolean;
  
  // Customização adicional
  className?: string;
  testID?: string;
}
```

### Exemplo de Uso Esperado

```tsx
// Exemplo básico
<CardComponent
  title="Título do Card"
  description="Descrição do card"
  size="md"
  variant="filled"
/>

// Exemplo com customização completa
<CardComponent
  title="Card Customizado"
  description="Com todas as opções"
  leftIcon={<Avatar src="..." />}
  rightIcon={<Icon name="arrow-right" />}
  titleColor="#FF5733"
  descriptionColor="#3498DB"
  leftIconColor="#2ECC71"
  rightIconColor="#9B59B6"
  backgroundColor="#F8F9FA"
  borderColor="#E74C3C" // ⚠️ Lembre-se desta prop!
  size="lg"
  variant="outlined"
  borderVariant="bordered"
  onPress={() => console.log('Card clicado')}
/>
```

## ✅ Critérios de Aceitação

1. ✅ Componente renderiza corretamente com todos os elementos opcionais
2. ✅ Cores individuais funcionam independentemente (título, descrição, ícones)
3. ✅ Todos os tamanhos são implementados e responsivos
4. ✅ Variantes de estilo funcionam corretamente
5. ✅ Customização de cor de fundo funciona
6. ✅ **Customização de cor de borda funciona (requisito crítico)**
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
9. **Testar customização de cor de borda em todas as variantes**
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

**Boa sorte no desenvolvimento! 🚀**

*Lembre-se: A customização da cor da borda é um requisito crítico que testa sua atenção aos detalhes!*

