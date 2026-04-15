# CLAUDE.md — BRASCONPE

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** BRASCONPE
**Nicho:** Educação
**Keywords:** Ola Sou a professora Marlene Dias e tambem fundadora deste maravilhoso blog
**Paleta de cores:** teal | **Fonte:** montserrat

Olá! Sou a professora Marlene Dias, e também fundadora deste maravilhoso blog. Adoro compartilhar meus conhecimentos e ajudar diversas pessoas com dicas e conteúdos 100% online a conseguir estudar ainda mais para seus objetivos. Acretido qua a Educação é o caminho para todos nós alcançarmos nossos objetivos e com isso tenho duas ambições: Auxiliar todos que estejam no objetivo de aprovação no enem ou no seu concurso dos sonhos de forma completamente gratuíta. Inovar com ideias criativas para educar crianças de eficar e alegre, construindo o conhecimento através do brincar. Sou formada em Letras e Pedagogia, tenho vasta experiencia nas escolas públicas do estado do Rio de janeiro e São Paulo, atuei por mais de 20 anos como professora Estadual. Amo estar na escola e no ambiente acadêmico! Mas acredito que a sala de aula não é possível para todos então venho atráves do meu blog passar todas as minhas vivencias e experiencias. “Escolha um trabalho que você ama e você nunca terá que trabalhar um dia sequer na vida”. Conhece essa frase? Ela me descreve totalmente!”



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-F |
| Hero | Hero-B |
| Features | Features-A |
| About Section | About-E |
| Posts | Posts-I |
| Footer | Footer-C |
| Página Sobre | Sobre-D |
| Página Contato | Contato-C |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
