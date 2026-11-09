# REDCODE – APK pelo GitHub

Desenvolvido por Josimar.

## Estrutura (como os arquivos devem ficar no repositório)

```
seu-repositorio/
├── .github/
│   └── workflows/
│       └── build-apk.yml
├── www/
│   └── index.html
├── .gitignore
├── capacitor.config.json
├── package.json
└── README.md
```

## Passo a passo

1. Crie um repositório novo no GitHub (pode ser privado).
2. Envie os arquivos: **Add file > Upload files**. Arraste `package.json`, `capacitor.config.json`, `.gitignore` e a pasta `www` (com o `index.html`).
3. O arquivo do workflow fica numa pasta oculta. Crie-o assim: **Add file > Create new file**, digite exatamente `.github/workflows/build-apk.yml` no nome e cole o conteúdo do arquivo `build-apk.yml`. Clique em **Commit changes**.
4. Abra a aba **Actions**. O build começa sozinho (ou clique em **Build APK > Run workflow**). Leva de 3 a 6 minutos.
5. Quando ficar verde, abra a execução e, em **Artifacts**, baixe **REDCODE-apk**. Dentro do zip está o `app-debug.apk`.
6. Passe o APK para o celular e instale. O Android vai pedir para permitir a instalação de fontes desconhecidas.

## Observações

- O progresso das lições fica salvo no aparelho e continua depois de fechar o app.
- Cada build gera uma assinatura nova. Para atualizar o app, desinstale a versão antiga antes (o progresso será apagado).
- Para mudar o app, edite o `www/index.html` no GitHub: um novo APK é gerado automaticamente.
