# Teste DevOps - Ivory IT

Este repositório contém o código e a configuração de uma pipeline CI/CD para o Teste Técnico – Estágio DevOps da Ivory IT. O objetivo deste projeto é implementar um fluxo automatizado para análise de código, versionamento e deploy de um site estático hospedado na AWS.

## Estrutura do Projeto

O projeto é composto pelos seguintes componentes principais:

Pipeline CI/CD: Configurada utilizando GitHub Actions, a pipeline inclui etapas de análise de código com SonarCloud, atualização do repositório no GitHub e deploy para o AWS S3.

Análise de Qualidade de Código: O código é analisado automaticamente através do SonarCloud para identificar vulnerabilidades, bugs e outros problemas de qualidade.

Deploy Automatizado: Após a análise, o código é automaticamente implantado em um bucket S3 da AWS, disponibilizando o site estático na web.

Site Estático: O projeto utiliza HTML e CSS para a criação de uma interface web simples e eficiente.

## Tecnologias Utilizadas
GitHub Actions: Para automação de CI/CD.

SonarCloud: Para análise de qualidade de código.

AWS S3: Para armazenamento e deploy do site estático.

HTML/CSS: Para construção da interface do site.

## Funcionamento da Pipeline

A pipeline é configurada para ser acionada sempre que um push é feito na branch main do repositório. A sequência das etapas da pipeline é a seguinte:

Checkout do código: A primeira etapa faz o checkout do código a partir do repositório GitHub.

Análise de Código: Em seguida, o código é analisado pelo SonarCloud, identificando possíveis vulnerabilidades e problemas de qualidade.

Deploy: Após a análise, o código é automaticamente implantado no bucket S3 da AWS, tornando o site acessível via URL pública.