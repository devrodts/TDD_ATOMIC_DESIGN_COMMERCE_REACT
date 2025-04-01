# TDD React Commerce

Este projeto implementa uma aplicação de e-commerce utilizando React com TypeScript, seguindo os princípios de Test-Driven Development (TDD) e a metodologia de design de componentes Atomic Design.

### Estrutura de diretórios

```
src/
  ├── assets/       # Recursos estáticos (imagens, ícones, etc.)
  ├── components/   # Componentes React (organizado com Atomic Design)
  │   ├── atoms/    # Componentes básicos e indivisíveis (botões, inputs, etc.)
  │   ├── celules/  # Agrupamento de componentes atômicos 
  │   ├── molecules/# Grupos funcionais de componentes simples
  │   ├── organism/ # Seções completas da interface
  │   └── templates/# Layouts de página
  ├── context/      # Contextos React para gerenciamento de estado global
  ├── hooks/        # Hooks React personalizados
  └── utils/        # Funções utilitárias e helpers
```

## Abordagens Utilizadas


### Test-Driven Development (TDD)

O TDD é uma metodologia de desenvolvimento onde:

- **Escrevemos testes antes do código**: Garantindo que os requisitos sejam bem compreendidos.
- **Seguimos o ciclo Red-Green-Refactor**: 
  1. Red: Escrever um teste que falha
  2. Green: Implementar o código mínimo para passar no teste
  3. Refactor: Melhorar o código mantendo os testes passando
- **Mantemos alta cobertura de testes**: Garantindo que todas as partes críticas da aplicação sejam testadas.
- **Facilitamos a refatoração**: Possibilitando mudanças com confiança de que nada foi quebrado.

### Atomic Design

O Atomic Design é uma metodologia para criação de sistemas de design que:

- **Divide componentes em níveis de complexidade**: Átomos, células, moléculas, organismos e templates.
- **Favorece a reutilização**: Componentes básicos são combinados para formar componentes mais complexos.
- **Mantém consistência**: Aplicação consistente de estilos e comportamentos em toda a interface.
- **Facilita manutenção**: Alterações em componentes básicos refletem em todos os lugares onde são usados.

## Benefícios da Arquitetura

1. **Manutenibilidade**: Código organizado por domínio facilita encontrar e modificar funcionalidades.
2. **Testabilidade**: Separação clara de responsabilidades torna os testes mais simples e focados.
3. **Escalabilidade**: Arquitetura modular permite expandir a aplicação com novos recursos sem afetar o código existente.
4. **Colaboração**: DDD facilita a comunicação entre equipes técnicas e não-técnicas.
5. **Qualidade**: TDD garante alta cobertura de testes e confiabilidade do código.
6. **Experiência consistente**: Atomic Design assegura uma interface de usuário coesa e previsível.


## Tecnologias Utilizadas

- React 19.0.0
- TypeScript
- Vite
- React Query para gerenciamento de estado assíncrono
- ESLint para garantir qualidade de código

## Como Iniciar

```bash
# Instalar dependências
yarn

# Iniciar o servidor de desenvolvimento
yarn dev

# Construir para produção
yarn build

# Executar verificação de lint
yarn lint
```
