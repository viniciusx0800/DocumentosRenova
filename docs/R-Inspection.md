# R-Inpection App 2.0

## Introduction

Sistema de vistoria veicular para as ECV-Empresas Credenciadas para Vistoria junto ao DETRAN, que executa uma análise completa do veículo em suas condições estruturais, identificação, histórico (roubo, furto, sinistros e leilão), pintura e itens acessórios, com a emissão do laudo de vistoria veicular, de forma integrada ao sistema RENAVAM. O sistema R Inspection é uma ferramenta completa que proporciona toda segurança para a compra de veículos seminovos de qualquer lugar do Brasil.

## Stack Version

- Android SDK: 33
- Node: 20.11.0
- Typescript: 5.1.3
- React Native: 0.72.6
- Expo: 49.0.21
- Redux: 8.1.2
- Java: 11.0.20

## Padrão de Branch

*tipo-da-branch/ número-da-tarefa - nome-da-branch*

feature/5451-adicao-funcionalidade

fix/5452-erro-x

hotfix/5453-correcao-em-producao

## Getting Started

Antes de iniciar, verifique se você possui as mesmas versões utilizadas no projeto.

1. **Processo de Instalação**
   1. Realize a instalação do node e java JDK
   2. Dentro do _root_ do projeto, execute a instalação das dependências `npm i`
2. **Conectar ao Expo**
   1. Execute o comando `npx expo login`
   2. Insira o email *suporte@renova.net.br* e senha `ed051209`
3. **Executar Projeto**
   1. Crie uma build do projeto, com o comando `npx expo run:android`
   2. Para iniciar o projeto, rode o comando `npx expo start --dev-client`
4. **Gerar APK**
   1. Execute o comando `eas build -p android --profile hmg`
5. **Limpar Cache (caso necessário)**
   1. Remova a pasta de `node_modules` e `android`
   2. Execute o comando de limpeza do cache no npm `npm cache clean --force`
   3. Reinstale as dependências com `npm i`
   4. Execute o comando de limpeza do expo `npx expo start --dev-client --clear`
6. **Placa de Testes**
   1. Em ambiente de Dev e Hmg deve-se usar a placa de testes do detran *JLE0A02*

## Informações Google

Para acessar serviços do Google, associados a esta aplicação, use o login abaixo.
A aplicação possui Firebase com serviço de crashlytics, analytics e log cadastrado.

1.  **Conta de acesso**
    1.  Email `renovamobile23@gmail.com`
    2.  Senha `Rnv@S0LUCO3S666`

2.  **Arquivos de Configuração**
    1.  Arquivo de configuração do Google IAM `./google-services.json`
    2.  Arquivo de configuração Firebase `./r-inspection-renova-468bc5465e73.json`    

## Features

1. Abertura de OS
2. Consulta OS
3. Vistoria de retorno
4. Suporte/Privacidade
5. Consulta Detran

## OTA Updates

**NECESSÁRIO TER EXTREMA CAUTELA E ATENÇÃO**

Atualizações de forma **direta nos usuários** da aplicação.
As atualizações OTA normalmente destinam-se à publicação de correções de pequenos bugs.

Não deve-se usar, em casos de inserção de pacotes!

1.  Execute um build da aplicação na **main**, usando `eas build -p android --profile main`.
2.  Realize o comando de _update_ da aplicação, inserindo uma mensagem descritiva
    `eas update --branch main --message "Mensagem descritiva"`
3.  Necessário reiniciar a aplicação uma ou duas vezes, a depender da quantidade de atualizações enviadas.

## Endpoints and Enviroment Variables:

.ENV localizadas no **root** do projeto `.\R-INSPECTION_APP_2.0_\.env`

- **.env Produção**
   
https://rinspection2-api.azurewebsites.net/api
- **.env Homologação**

https://rinspection2-api-hmg.azurewebsites.net/api
- **.env Desenvolvimento**

https://rinspection2-api-dev.azurewebsites.net/api
- **.env PRIVACIDADE**

https://api.whatsapp.com/send/?phone=5571999403953&text=Ol%C3%A1&type=phone_number&app_absent=0
- **.env PRIVACIDADE**

https://renova.net.br/site/1380-2/