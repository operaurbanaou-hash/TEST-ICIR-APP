# ICIR APP

Projeto Android externo do **Minha ICIR**, preparado para gerar um APK instalável diretamente no Android, sem depender da aprovação da Play Store.

- App: Minha ICIR
- Application ID: `br.com.ministerioicir.minhaicir`
- Versão: `1.0.1`
- Site/app web atual: `https://icirtest.operaurbana.arq.br/?app=1`

O workflow em `.github/workflows/build-external-apk.yml` gera automaticamente o artefato `MinhaICIR-External-v1.0.1.apk` a cada push na branch `main`.

> Observação: este repositório é público. A chave privada de assinatura externa não é enviada ao GitHub. O build automático atual usa `assembleDebug`, adequado para instalação e testes externos. Para distribuição estável com atualizações futuras usando a mesma assinatura, a chave deve ser configurada de forma privada (por exemplo, como GitHub Secret em repositório privado ou em ambiente seguro).
