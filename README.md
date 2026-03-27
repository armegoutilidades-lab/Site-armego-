# Site Armego - DropShip Brasil

Website institucional da Armego Utilidades com integração do Vercel Speed Insights.

## 🚀 Características

- Site estático responsivo
- Integração com Vercel Speed Insights para monitoramento de performance
- Estilização customizada com tema azul e laranja

## 📦 Tecnologias

- HTML5
- CSS3 (style.css)
- Vercel Speed Insights

## 🔧 Instalação

```bash
# Instalar dependências
npm install

# Executar localmente
npm run dev
```

## 🌐 Deploy

Este projeto está configurado para deploy automático na Vercel. O Speed Insights será ativado automaticamente após o deploy.

### Configurando Speed Insights na Vercel

1. Acesse o [Dashboard da Vercel](https://vercel.com/dashboard)
2. Selecione seu projeto
3. Vá para **Speed Insights** no menu lateral
4. Clique em **Enable** para ativar o monitoramento

Após o deploy, os dados de performance começarão a aparecer no dashboard dentro de alguns dias.

## 📊 Speed Insights

O Vercel Speed Insights está integrado diretamente no `index.html`:

```html
<script>
  window.si = window.si || function () { (window.siq = window.siq || []).push(arguments); };
</script>
<script defer src="/_vercel/speed-insights/script.js"></script>
```

Este script rastreia métricas de performance como:
- First Contentful Paint (FCP)
- Largest Contentful Paint (LCP)
- Cumulative Layout Shift (CLS)
- First Input Delay (FID)
- Time to First Byte (TTFB)

## 📁 Estrutura do Projeto

```
.
├── index.html          # Página principal
├── style.css           # Estilos personalizados
├── vercel.json         # Configuração da Vercel
├── package.json        # Dependências e scripts
└── README.md           # Documentação
```

## 📄 Licença

ISC
