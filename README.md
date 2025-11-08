# Portfolio 2025 - Gustavo Francisco

Um portfolio moderno e responsivo desenvolvido com Next.js, React e TypeScript para showcase de projetos Full Stack.

## 🚀 Tecnologias Utilizadas

- **Frontend**: Next.js 15, React 19, TypeScript
- **Estilização**: CSS Modules com design responsivo
- **Carrossel**: Embla Carousel para galerias de imagens
- **Otimização**: Next.js Image Optimization com suporte a WebP/AVIF
- **Fontes**: Google Fonts (Geist)
- **Metadados**: SEO otimizado com OpenGraph e Twitter Cards

## 📱 Funcionalidades

### Página Principal
- Hero section com apresentação pessoal
- Navegação intuitiva entre seções
- Design responsivo para todos os dispositivos

### Seção Sobre Mim
- Foto de perfil profissional
- Descrição detalhada sobre experiência e habilidades
- Showcase de tecnologias com ícones animados
- Links para redes sociais e contato
- Botão para download do currículo

### Seção de Projetos
- Galeria interativa com projetos dinâmicos carregados do JSON
- Sistema de filtragem por tecnologias
- Cards de projetos com imagens e descrições
- Modal de galeria com carrossel de imagens
- Links diretos para projetos e repositórios
- Organização por projetos em destaque (featured)

### Sistema de Galeria
- Context API para gerenciamento de estado
- Carrossel com navegação por setas e dots
- Legendas descritivas para cada imagem
- Suporte a múltiplos formatos de imagem
- Otimização de carregamento com lazy loading

## 🛠️ Estrutura do Projeto

```
src/
├── app/
│   ├── components/          # Componentes reutilizáveis
│   │   ├── carouselPage/   # Carrossel de páginas
│   │   ├── carouselText/   # Carrossel de texto
│   │   ├── projectCard/    # Card individual de projeto
│   │   ├── projectFilter/  # Filtro de projetos
│   │   ├── projectGallery/ # Galeria de imagens
│   │   ├── projectGrid/    # Grid de projetos
│   │   └── embla-*         # Componentes Embla Carousel
│   ├── contexts/           # Context API
│   │   └── GalleryContext.tsx
│   ├── pages/              # Páginas principais
│   │   ├── about/          # Sobre mim
│   │   ├── projects/       # Projetos
│   │   ├── certifications/ # Certificações
│   │   └── experiences/    # Experiências
│   ├── globals.css         # Estilos globais
│   ├── layout.tsx          # Layout principal
│   └── page.tsx            # Página inicial
├── data/
│   └── projects.json       # Dados dos projetos
└── public/
    └── assets/             # Recursos estáticos
        ├── icons/          # Ícones
        ├── screenshots/    # Screenshots dos projetos
        ├── techs/          # Ícones de tecnologias
        └── profile.jpg     # Foto de perfil
```

## 📊 Dados dos Projetos

Os projetos são armazenados em `src/data/projects.json` com a seguinte estrutura:

```json
{
  "id": "identificador-unico",
  "title": "Título do Projeto",
  "subtitle": "Tecnologias Principais",
  "description": "Descrição detalhada...",
  "images": ["/assets/screenshots/projeto/img1.png"],
  "captions": ["Legenda da imagem"],
  "link": "https://url-do-projeto.com",
  "canVisit": true,
  "tags": ["tecnologia1", "tecnologia2"],
  "featured": true
}
```

## 🚀 Instalação e Execução

### Pré-requisitos
- Node.js 18+ 
- npm ou yarn

### Passos

1. **Clone o repositório**
   ```bash
   git clone https://github.com/ciscosweater/portfolio2025.git
   cd portfolio2025
   ```

2. **Instale as dependências**
   ```bash
   npm install
   ```

3. **Inicie o servidor de desenvolvimento**
   ```bash
   npm run dev
   ```

4. **Acesse no navegador**
   ```
   http://localhost:3000
   ```

### Scripts Disponíveis

```bash
npm run dev      # Inicia servidor de desenvolvimento
npm run build    # Build para produção
npm run start    # Inicia servidor de produção
npm run lint     # Executa ESLint
```

## 🎨 Design e Estilização

### Principais Características
- **Design Responsivo**: Adaptado para mobile, tablet e desktop
- **Performance**: Otimizado com Next.js Image e lazy loading
- **Acessibilidade**: Semântica HTML5 e navegação por teclado
- **Animações**: Transições suaves e micro-interações
- **Tema**: Design moderno com cores profissionais

### Paleta de Cores
- Cores neutras com contraste adequado
- Destaque em elementos interativos
- Background clean para melhor leitura

## 📈 SEO e Performance

### Otimizações
- **Metadados**: OpenGraph, Twitter Cards, schema.org
- **Imagens**: Formatos WebP/AVIF, lazy loading, responsive images
- **Fontes**: Google Fonts com otimização
- **Cache**: Estratégias de cache estático
- **Core Web Vitals**: Otimizado para LCP, FID, CLS

### Ferramentas Utilizadas
- Next.js SEO optimizations
- Image optimization pipeline
- Automatic sitemap generation
- Robots.txt configuration

## 🔧 Configuração

### Variáveis de Ambiente
O projeto não requer variáveis de ambiente para funcionar localmente.

### Configuração do Next.js
```typescript
// next.config.ts
const nextConfig: NextConfig = {
  images: {
    formats: ['image/webp', 'image/avif'],
    deviceSizes: [640, 750, 828, 1080, 1200, 1920],
    imageSizes: [16, 32, 48, 64, 96, 128, 256, 384],
    minimumCacheTTL: 60,
  },
};
```

## 📱 Projetos em Destaque

O portfolio showcase projetos dinâmicos carregados do arquivo `src/data/projects.json`. 

Os projetos são organizados automaticamente com:
- **Projetos em destaque** (featured: true) exibidos primeiramente
- **Filtragem por tecnologias** baseada nas tags
- **Galeria de imagens** com captions descritivas
- **Links diretos** para demonstrações e repositórios

### Estrutura Dinâmica
A lista de projetos é atualizada automaticamente conforme o arquivo JSON, permitindo fácil manutenção e adição de novos projetos sem necessidade de modificar o README.

## 🤝 Contribuição

Para adicionar novos projetos, siga o guia em [COMO_ADICIONAR_PROJETOS.md](./COMO_ADICIONAR_PROJETOS.md).

### Passos Rápidos
1. Adicione screenshots em `public/assets/screenshots/`
2. Configure o projeto em `src/data/projects.json`
3. Teste localmente com `npm run dev`

## 📄 Licença

Este projeto é para uso pessoal e demonstração das habilidades do desenvolvedor.

## 📞 Contato

- **Email**: gustavo.f6041@gmail.com
- **GitHub**: [ciscosweater](https://github.com/ciscosweater)
- **Portfolio**: [gustavo-francisco.vercel.app](https://gustavo-francisco.vercel.app)

---

Desenvolvido com ❤️ por Gustavo Francisco