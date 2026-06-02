# Terminal-DiamanteBlack — Projeto Capacitor Android

Gerado automaticamente pelo **DiamantePink PWA Builder** 💎

## 📱 Como gerar o APK

### Opção 1: Via GitHub Actions (RECOMENDADO — gratuito, sem instalar nada)

1. Crie um repositório no GitHub (ou use um existente)
2. Faça upload de todos os arquivos deste ZIP para o repositório
3. O workflow em `.github/workflows/build-apk.yml` será executado automaticamente
4. Após ~5 minutos, vá em **Actions → Build APK → Artefatos**
5. Baixe o arquivo `terminaldiamanteblac-debug-apk.zip` — dentro estará o `.apk`

### Opção 2: Localmente com Android Studio

**Pré-requisitos:**
- Node.js 18+
- Android Studio instalado
- Android SDK API 34

**Passos:**
```bash
# 1. Instalar dependências
npm install

# 2. Sincronizar com Android
npx cap sync android

# 3. Abrir no Android Studio
npx cap open android

# 4. No Android Studio: Build → Build Bundle(s)/APK(s) → Build APK(s)
# O APK ficará em: android/app/build/outputs/apk/debug/app-debug.apk
```

### Opção 3: Linha de comando (sem Android Studio)

```bash
npm install
npx cap sync android
cd android
./gradlew assembleDebug
# APK em: app/build/outputs/apk/debug/app-debug.apk
```

## 📦 Informações do App

| Campo         | Valor             |
|---------------|-------------------|
| Nome          | Terminal-DiamanteBlack        |
| Package ID    | br.diamantepink.terminaldiamanteblac          |
| Version       | 1.0.0             |
| Min Android   | API 22 (5.1+)     |
| Target        | API 34 (Android 14)|

## 🔐 Permissões configuradas

- `INTERNET` — acesso à rede
- `CAMERA` — câmera (se usada pelo app)
- `READ/WRITE_EXTERNAL_STORAGE` — arquivos
- `RECORD_AUDIO` — microfone (se usado pelo app)
- `VIBRATE` — vibração

---
*Gerado pelo DiamantePink v5.0 — 01/06/2026*
