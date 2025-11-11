# Website do Curso de Ciência de Dados e Inteligência Artificial - UFPB

Site institucional do Bacharelado em Ciência de Dados e Inteligência Artificial da Universidade Federal da Paraíba, desenvolvido com Jekyll para hospedagem no GitHub Pages.

## Características

- Design moderno e responsivo
- Paleta de cores profissional
- Navegação intuitiva
- Otimizado para dispositivos móveis
- SEO otimizado
- Carregamento rápido

## Requisitos

- Ruby 2.7 ou superior
- Jekyll 4.3
- Bundler

## Instalação

### Opção 1: Deploy Direto no GitHub Pages (Recomendado - Mais Fácil)

Não requer instalação local! Basta fazer push para o GitHub e ativar o GitHub Pages.

**Vantagens:**
- Sem necessidade de instalar Ruby/Jekyll localmente
- Deploy automático
- Hospedagem gratuita
- SSL/HTTPS incluído

Veja o arquivo [INSTALL.md](INSTALL.md) para instruções detalhadas.

### Opção 2: Instalação Local (Para desenvolvimento)

Para testar o site localmente:

1. **Instale as ferramentas de desenvolvimento**
   - macOS: `xcode-select --install`
   - Linux: `sudo apt-get install ruby-full build-essential`
   - Windows: Instale [RubyInstaller](https://rubyinstaller.org/)

2. **Clone e instale**
   ```bash
   git clone [url-do-repositorio]
   cd cdia-website
   bundle install
   ```

3. **Execute o servidor**
   ```bash
   bundle exec jekyll serve
   ```

4. **Acesse**
   ```
   http://localhost:4000
   ```

**Problemas na instalação?** Consulte [INSTALL.md](INSTALL.md) para soluções ou [TROUBLESHOOTING.md](TROUBLESHOOTING.md) se encontrar erros específicos.

## Estrutura do Projeto

```
cdia-website/
├── _config.yml          # Configurações do Jekyll
├── _includes/           # Componentes reutilizáveis (header, footer)
├── _layouts/            # Templates de páginas
├── _sass/               # Arquivos SCSS
├── assets/
│   ├── css/            # CSS compilado
│   ├── js/             # JavaScript
│   └── images/         # Imagens
├── _noticias/          # Posts de notícias
├── index.html          # Página inicial
└── [outras páginas].md # Páginas do site
```

## Personalização

### Cores

As cores podem ser alteradas no arquivo `_sass/_variables.scss`:

- `--color-primary`: Cor principal (azul)
- `--color-accent`: Cor de destaque (azul claro/verde)
- `--color-accent-warm`: Cor de destaque quente (laranja)

### Navegação

O menu de navegação é configurado em `_config.yml` na seção `navigation`.

### Conteúdo

- **Páginas**: Edite os arquivos `.md` na raiz do projeto
- **Notícias**: Adicione arquivos em `_noticias/`
- **Configurações gerais**: `_config.yml`

## Deploy no GitHub Pages

1. Faça commit das alterações:
```bash
git add .
git commit -m "Atualização do site"
```

2. Envie para o GitHub:
```bash
git push origin main
```

3. Ative o GitHub Pages nas configurações do repositório:
   - Settings > Pages
   - Source: Deploy from branch
   - Branch: main / (root)

O site estará disponível em: `https://[seu-usuario].github.io/[nome-do-repo]`

## Adicionando Conteúdo

### Nova Página

Crie um arquivo `.md` na raiz:

```markdown
---
layout: page
title: Título da Página
subtitle: Subtítulo opcional
---

Conteúdo da página em Markdown...
```

### Nova Notícia

Crie um arquivo em `_noticias/` com o formato `YYYY-MM-DD-titulo.md`:

```markdown
---
layout: post
title: Título da Notícia
date: 2024-01-15
---

Conteúdo da notícia...
```

## Suporte

Para dúvidas ou problemas, abra uma issue no repositório.

## Licença

Este projeto é desenvolvido para uso institucional da UFPB.
