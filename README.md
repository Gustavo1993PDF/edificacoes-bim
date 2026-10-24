# Edificações BIM

Painel demonstrativo, em português, para explorar um fluxo de informações de uma edificação: modelo 3D, terreno, estruturas e quantitativos. O projeto é uma experiência independente e leve, feita para funcionar diretamente no navegador, sem backend ou dependências de build.

## O que está incluído

- Navegação de página única entre **Visão geral**, **Modelo 3D**, **Mapa**, **Estruturas**, **Quantitativos** e **Configurações**.
- Dados locais demonstrativos para cartões de métricas, atividades, camadas e propriedades de elementos.
- Visualizações ilustrativas de modelo federado, sistema estrutural e implantação no terreno.
- Seleção de camadas, painel de propriedades, filtros de quantitativos, preferências e feedbacks interativos.
- Layout responsivo para desktop, tablet e celular, com navegação móvel.

Os dados e visualizações são intencionalmente demonstrativos. O painel não salva informações e não se conecta a um servidor.

## Executar localmente

Como o site é estático, basta abrir `index.html` no navegador. Para simular um servidor local (recomendado para testar o comportamento completo), use qualquer servidor HTTP, por exemplo:

```bash
python -m http.server 8000
```

Depois, acesse <http://localhost:8000>.

## Publicar no GitHub Pages

O workflow `.github/workflows/pages.yml` publica automaticamente o conteúdo do repositório no GitHub Pages a cada push na branch `main`.

1. No repositório, abra **Settings → Pages**.
2. Em **Build and deployment**, escolha **GitHub Actions** como fonte.
3. Faça push para `main` ou execute manualmente o workflow **Publicar no GitHub Pages** na aba **Actions**.

O workflow envia o repositório como um site estático, sem etapa de compilação.
