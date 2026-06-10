# 📚 Guia de Documentação - Português

Bem-vindo ao guia de documentação do **AgroVision**! Este documento explica como estruturar, escrever e manter a documentação do projeto.

## Índice

- [Estrutura de Documentação](#estrutura-de-documentação)
- [Padrões de Escrita](#padrões-de-escrita)
- [Tipos de Documentação](#tipos-de-documentação)
- [Boas Práticas](#boas-práticas)
- [Versionamento de Docs](#versionamento-de-docs)

## Estrutura de Documentação

### Hierarquia de Pastas

```
docs/
├── README.md                 # Índice da documentação
├── getting-started.pt.md     # Guia de início (PT)
├── data-guide.pt.md          # Guia de dados (PT)
├── documentation-guide.pt.md # Este documento
├── api/
│   ├── endpoints.md
│   └── authentication.md
├── guides/
│   ├── setup.md
│   └── deployment.md
└── tutorials/
    ├── first-analysis.md
    └── data-visualization.md
```

## Padrões de Escrita

### 1. Estrutura de Títulos

Sempre use Markdown headers consistentemente:

```markdown
# Título Principal (H1)
## Seção (H2)
### Subsection (H3)
#### Detalhes (H4)
```

### 2. Tone and Voice (Tom e Voz)

- **Amigável**: Use linguagem acessível
- **Claro**: Evite jargão técnico sem explicação
- **Conciso**: Vá direto ao ponto
- **Inclusivo**: Considere públicos diversos (agricultores, pesquisadores, etc.)

### 3. Formatação

Use markdown de forma consistente:

```markdown
- **Negrito** para termos importantes
- `code` para nomes de arquivo/função
- [Links](url) para referências
- > Citações para destaque
- ```code blocks``` para exemplos
```

## Tipos de Documentação

### 1. Documentação de Início Rápido

**Objetivo**: Fazer o usuário começar em 5 minutos

**Exemplo estrutura**:
- Pré-requisitos
- Instalação
- Primeiro uso
- Próximos passos

### 2. Guias How-To

**Objetivo**: Resolver um problema específico

**Exemplo estrutura**:
- Problema
- Solução passo a passo
- Exemplos práticos
- Dicas e truques

### 3. Referência

**Objetivo**: Documentação completa de APIs/funções

**Exemplo estrutura**:
- Descrição
- Parâmetros
- Exemplos de uso
- Casos de erro

### 4. Explicações Conceituais

**Objetivo**: Educação sobre ideias/conceitos

**Exemplo estrutura**:
- Contexto
- Explicação detalhada
- Exemplos reais
- Recursos adicionais

## Boas Práticas

### 1. Escreva para o Público

Considere quem está lendo:

- **Para Agricultores**: Use exemplos práticos, evite jargão muito técnico
- **Para Pesquisadores**: Inclua referências científicas, metodologia
- **Para Desenvolvedores**: Use exemplos de código, detalhes técnicos
- **Para Comunidade Geral**: Linguagem simples e acessível

### 2. Use Exemplos Reais

```markdown
❌ Ruim: "Insira os dados"
✅ Bom: "Copie suas dados CSV para a pasta `data/raw/` e execute:"
```

### 3. Mantenha Documentação Atualizada

- Atualize docs quando o código muda
- Verifique links regularmente
- Revise e melhore continuamente

### 4. Incluya Imagens e Diagramas

```markdown
![Descrição da Imagem](caminho/para/imagem.png)
```

### 5. Use Tabelas para Comparações

```markdown
| Recurso | Descrição | Audiência |
|---------|-----------|-----------|
| Data Guide | Como trabalhar com dados | Todos |
| API Ref | Referência técnica | Desenvolvedores |
```

### 6. Adicione Avisos e Dicas

```markdown
> **⚠️ Aviso**: Certifique-se de fazer backup primeiro
> **💡 Dica**: Use variáveis de ambiente para senhas
> **ℹ️ Nota**: Esta feature está em beta
```

## Versionamento de Docs

### Manutenção de Versões

1. **Docs Principais**: Sempre refletem a versão mais recente
2. **Docs de Release**: Arquivadas por versão se necessário
3. **Changelog**: Registre mudanças importantes na documentação

### Quando Atualizar

- Novos recursos
- Mudanças de API
- Correções de bugs
- Melhorias de performance
- Mudanças de estrutura

## Revisão de Documentação

### Checklist para Pull Requests

- [ ] Títulos claros e descritivos
- [ ] Exemplos funcionais e testados
- [ ] Links funcionam corretamente
- [ ] Formatação consistente
- [ ] Revisão por outro mantenedor
- [ ] Sem erros de digitação

## Recursos Adicionais

- 📖 [Documentação Completa](../README.pt.md)
- 🤝 [Contribuindo](../CONTRIBUTING.md)
- 💬 [Discussões](../../discussions)

---

**Versões em outros idiomas:** [🇬🇧 English](./documentation-guide.en.md) | [🇪🇸 Español](./documentation-guide.es.md)

Tem dúvidas sobre documentação? [Abra uma Discussion](../../discussions)
