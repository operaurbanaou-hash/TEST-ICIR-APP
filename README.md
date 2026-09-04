# ICIR APP

Projeto Android externo do **Minha ICIR**, preparado para gerar um APK instalável diretamente no Android, sem depender da aprovação da Play Store.

- App: Minha ICIR
- Application ID: `br.com.ministerioicir.minhaicir`
- Versão: `1.0.1`
- Site/app web atual: `https://icirtest.operaurbana.arq.br/?app=1`
- Fonte Android: `ICIR-APP-SOURCE.zip`

O workflow em `.github/workflows/build-external-apk.yml` extrai o projeto e gera automaticamente o artefato `MinhaICIR-External-v1.0.1.apk` a cada push na branch `main` ou por execução manual.

## Segurança da assinatura

Este repositório é público. Por isso, a chave privada de assinatura externa e suas senhas **não foram enviadas ao GitHub**. O build automático atual usa `assembleDebug`, adequado para instalação e testes externos.

Para uma distribuição estável com atualizações futuras assinadas sempre pela mesma chave, a chave deve permanecer privada e ser configurada em ambiente seguro antes do build de release.
