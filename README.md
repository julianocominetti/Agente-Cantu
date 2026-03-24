# 🌿 Agente Cantu — Deploy no Vercel

## Arquivos necessários
```
/
├── index.html     ← agente completo (UI + lógica)
└── vercel.json    ← configuração Vercel
```

## Deploy em 3 passos

### 1. Crie um repositório no GitHub
- Acesse github.com/new
- Nomeie o repositório (ex: `agente-cantu`)
- Faça upload dos dois arquivos: `index.html` e `vercel.json`

### 2. Deploy no Vercel
- Acesse vercel.com e faça login (pode usar a conta GitHub)
- Clique em **"Add New Project"**
- Selecione o repositório `agente-cantu`
- Framework Preset: **Other**
- Clique em **Deploy**

### 3. Configure a OpenAI API Key no app
- Acesse a URL gerada pelo Vercel (ex: `agente-cantu.vercel.app`)
- No painel lateral esquerdo, cole sua **OpenAI API Key** (`sk-...`)
- Clique em **Salvar Chave**
- A chave fica salva no `localStorage` do navegador — não sai para o servidor

## Como usar
1. Com a API Key salva, clique em **"Iniciar Agente & Carregar Base"**
2. O agente carrega automaticamente a base do GitHub
3. O panorama geral é exibido automaticamente
4. Use o menu lateral ou o chat livre para navegar pelas análises

## Funcionalidades
- ✅ Panorama geral de todas as filiais
- ✅ Análise completa por filial (opção 1)
- ✅ Clientes por filial (opção 2)
- ✅ Categorias por filial (opção 3)
- ✅ Ranking clientes da rede (opção 4)
- ✅ Ranking categorias da rede (opção 5)
- ✅ Margem por filial (opção 6)
- ✅ Projeção consolidada do grupo (opção 7)
- ✅ Análise livre (opção 8)
- ✅ Regra Celso Ramos + Cristal Verde automática
- ✅ Cálculo de projeção baseado na data atual do sistema
- ✅ Formatação com sinalizações ⚠️ 🔴 🔄 🔍

## Segurança
A API Key é armazenada apenas no `localStorage` do seu navegador.
Ela nunca passa por nenhum servidor intermediário — vai direto para a OpenAI.

## Atualização da base
Para atualizar os dados, basta atualizar o arquivo `base_cantu_IA.txt` no repositório:
`https://github.com/julianocominetti/Agente-Cantu`
O agente sempre lê a versão mais recente ao iniciar.
