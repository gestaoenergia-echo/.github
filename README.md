# Bem-vindo à Gestão de Energia da Echoenergia! ⚡

Esta é a organização oficial no GitHub para os projetos, ferramentas e códigos utilizados pela área de **Gestão de Energia da Echoenergia**.

Nosso objetivo é facilitar a colaboração entre as equipes, reutilizar soluções e preservar o conhecimento técnico da área.

---

## 🗂️ Organização dos projetos

Cada repositório deve representar um **produto, processo ou projeto com finalidade própria**. Não deve ser criado um repositório para cada script, nem um único repositório para todos os códigos da área.

Exemplos de nomes: `aymore`, `meridian`, `curva-forward` e `precificacao`.

Um novo repositório deve ter objetivo claro, documentação própria e uma equipe responsável. Projetos que fazem parte do mesmo processo, mudam juntos e possuem os mesmos responsáveis podem permanecer no mesmo repositório.

---

## 📁 Estrutura de cada repositório

Cada projeto deve começar com uma estrutura simples:

```text
nome-do-projeto/
├── README.md
├── codigos/
├── configuracoes/     ← somente se precisar
├── testes/            ← somente quando existirem
├── requirements.txt
└── .gitignore
```

- **`README.md`**: apresenta o objetivo, a equipe responsável, as fontes utilizadas e as instruções de execução.
- **`codigos/`**: contém os scripts do projeto.
- **`configuracoes/`**: contém parâmetros que podem ser alterados sem modificar a lógica do código.
- **`testes/`**: contém as verificações automáticas do projeto.
- **`requirements.txt`**: relaciona as bibliotecas Python necessárias.
- **`.gitignore`**: identifica os arquivos que não devem ser enviados ao GitHub.

Não é necessário criar pastas vazias. Bases operacionais, resultados temporários, arquivos de log, senhas, tokens e credenciais não devem ser armazenados no GitHub.

---

## ✍️ Padrão de nomes

### Repositórios

- Utilizar nomes em português, sempre que possível.
- Utilizar letras minúsculas e sem acentos.
- Separar as palavras com hífen.
- Evitar números usados apenas para forçar uma ordem.
- Evitar nomes genéricos como `diversos`, `outros`, `novo` ou `testes`.

Exemplos: `aymore`, `meridian`, `curva-forward` e `precificacao`.

### Pastas

- Utilizar letras minúsculas e sem acentos.
- Separar as palavras com sublinhado.
- Criar novas pastas somente quando seu conteúdo justificar a existência.

### Scripts Python

Os scripts devem começar pela origem principal da informação, seguida da ação e do conteúdo:

```text
<origem>_<acao>_<conteudo>_<detalhe_opcional>.py
```

A origem pode ser uma fonte de dados, sistema, modelo ou processo interno, como `ons`, `ccee`, `bbce`, `psr`, `thunders`, `newave`, `decomp`, `dessem`, `interno` ou `multifonte`.

```text
interno_calcular_preco_modulacao.py
multifonte_consolidar_curva_forward.py
ons_ccee_comparar_decks_newave.py
```

A ação deve ser escrita no infinitivo, como `coletar`, `processar`, `atualizar`, `calcular`, `consolidar`, `comparar`, `validar`, `gerar` ou `enviar`.

Termos como `diaria`, `mensal` e `horaria` devem representar a granularidade da informação, e não apenas a frequência de execução.

Não utilizar nomes de pessoas, datas ou versões, como `codigo_nathalia.py`, `atualizacao_2026.py` ou `versao_final_v2.py`. O histórico de versões deve ser mantido pelo GitHub.

---

## 👥 Responsabilidade pelos projetos

Cada repositório deve ficar sob a responsabilidade de uma **equipe**, e não de uma única pessoa. A equipe deve ter pelo menos dois integrantes com conhecimento e acesso ao projeto.

O `README.md` de cada repositório deve informar a equipe responsável. Se alguém sair da empresa ou mudar de função, os administradores atualizam os integrantes da equipe sem interromper a continuidade do projeto.

Para reduzir o risco de perda de acesso, a organização deve manter pelo menos dois administradores.
