# Gabinete do Professor (Electron)

Esta pasta contém a wrapper Electron para transformar a app web num aplicativo desktop.

## Como usar

1. Instalar dependências

```bash
npm install
```

2. Executar em modo de desenvolvimento

```bash
npm run start
```

3. Gerar pacotes instaláveis

```bash
npm run dist
```

Os artefactos de build serão colocados em `dist/`.

Observações:
- O service worker do PWA não será registado quando a app correr em `file://` dentro do Electron — isso é normal e não impede o funcionamento desktop.
- Para criar builds macOS assinados é recomendado executar `npm run dist` em macOS. Windows/Linux geram .exe/.AppImage/.deb conforme o ambiente.

Se quiser, posso também adicionar um workflow GitHub Actions para gerar os builds automaticamente quando fizer push ou ao criar uma tag.
