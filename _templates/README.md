# Templates de Perfil — Observatório Oceanográfico (O₂)

Este diretório contém **templates oficiais** para a criação de páginas individuais de colaboradores do **Observatório Oceanográfico da UFF**.

Esses templates servem como ponto de partida para que cada integrante do O₂ possa criar seu próprio perfil no site institucional, em **português e/ou inglês**, seguindo um padrão consistente.

---

## 📌 Fluxo de trabalho (importante)

O processo correto para criar ou atualizar seu perfil é:

1. **Faça um fork** deste repositório para a sua conta GitHub
2. **Copie** o template adequado deste diretório
3. **Edite apenas os arquivos do seu perfil**
4. **Envie um Pull Request (PR)** para o repositório principal
5. A coordenação do O₂ fará a revisão e integração

> ❗ **Não edite diretamente os arquivos deste diretório `_templates/`.**  
> Eles existem apenas como referência.

---

## 📁 Onde criar seu perfil

Após copiar o template, coloque os arquivos nos seguintes diretórios: **Português**  `_people/pt/` e **Inglês** `_people/en/`. O nome do arquivo deve seguir o padrão `nome-sobrenome.md` (por exemlplo: `andre-belem.md`, nada de maiúsculas, nada de acentos e use o hífen `-`).

## 📝 O que você deve editar no template

No início do arquivo (front matter), você verá vários campos.  
Abaixo está uma explicação dos **principais campos obrigatórios**:

### 🔹 Campos obrigatórios
- `title` — seu nome completo
- `lang` — idioma do arquivo (`pt` ou `en`)
- `permalink` — URL do seu perfil
- `role` — sua função/cargo acadêmico
- `avatar` — caminho para sua foto
- `order` — número que define a ordem na página da equipe

### 🔹 Campos opcionais (preencha apenas se tiver)
- `affiliation` / `affiliation_url`
- `email`
- `github`
- `orcid`
- `scholar`
- `lattes` (apenas na versão em português)
- `scopus`
- `medium`
- `location`

> ⚠️ **Nunca remova campos estruturais**, mesmo que não vá usá-los.  
> Se não tiver a informação, deixe o campo vazio ou remova apenas a linha correspondente.

---

## 🖼️ Sobre a foto (`avatar`)

- A imagem deve ser **quadrada (proporção 1:1)**
- Formatos aceitos: `.jpg` ou `.png`
- Coloque a imagem em `## 📝 O que você deve editar no template

No início do arquivo (front matter), você verá vários campos.  
Abaixo está uma explicação dos **principais campos obrigatórios**:

### 🔹 Campos obrigatórios
- `title` — seu nome completo
- `lang` — idioma do arquivo (`pt` ou `en`)
- `permalink` — URL do seu perfil
- `role` — sua função/cargo acadêmico
- `avatar` — caminho para sua foto
- `order` — número que define a ordem na página da equipe

### 🔹 Campos opcionais (preencha apenas se tiver)
- `affiliation` / `affiliation_url`
- `email`
- `github`
- `orcid`
- `scholar`
- `lattes` (apenas na versão em português)
- `scopus`
- `medium`
- `location`

> ⚠️ **Nunca remova campos estruturais**, mesmo que não vá usá-los.  
> Se não tiver a informação, deixe o campo vazio ou remova apenas a linha correspondente.

---

## 🖼️ Sobre a foto (`avatar`)

- A imagem deve ser **quadrada (proporção 1:1)**
- Formatos aceitos: `.jpg`
- Coloque a imagem em: `assets/img/people/` usando o mesmo esquema do arquivo pessoal (Ex: `nome-sobrenome.jpg`)

---

## ✍️ Texto de apresentação

Após o front matter, escreva um texto curto de apresentação.

Sugestões:
- sua formação
- área de atuação
- interesses de pesquisa
- projetos atuais

Não é necessário escrever muito.  
**Um parágrafo claro já é suficiente.**

Se preferir, pode deixar o texto provisório — ele pode ser revisado depois.

---

## 🌍 Perfis em dois idiomas

- Se você criar **apenas um idioma**, tudo bem
- Se criar **português e inglês**, lembre-se de:
- ajustar corretamente o campo `alt_lang`
- usar o mesmo nome de arquivo (em pastas diferentes)

Exemplo: `_people/pt/nome-sobrenome.md` ou `_people/en/nome-sobrenome.md`

---

## ⚠️ Erros comuns (evite!)

- ❌ Esquecer de fechar aspas (`"`)
- ❌ Usar caracteres especiais sem aspas (`·`, `:`)
- ❌ Alterar arquivos fora do seu perfil
- ❌ Editar arquivos dentro de `_templates/`
- ❌ Usar fotos muito grandes ou fora de proporção
- ❌ Esquecer de colocar o seu lattes ou o email institucional.

Se algo não aparecer no site, o problema geralmente é **algum código inválido no seu texto**.

---

## 🤝 Enviando o Pull Request

Antes de enviar o PR:
- verifique se o site compila corretamente no seu fork
- confira se o link do seu perfil funciona
- revise erros de digitação

No texto do PR, descreva brevemente:
- quem você é
- o que foi alterado
- se o perfil está completo ou provisório

---

## 📬 Dúvidas?

Em caso de dúvidas:
- consulte este README
- olhe outros perfis já publicados (principalmente o da F.R.I.D.A.Y.)
- ou entre em contato com a coordenação do Observatório Oceanográfico

Bem-vindo(a) ao O₂! 🌊
