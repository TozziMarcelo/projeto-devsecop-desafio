# Desafio DevSecOps — Gerenciador de Tarefas

## Sobre o Projeto
Este repositório faz parte do desafio prático do módulo de DevSecOps da ADA Tech.
Você receberá este projeto com vulnerabilidades propositais e uma pipeline incompleta.
Seu objetivo é **implementar a pipeline de segurança** e **corrigir as vulnerabilidades**.

## Estado atual
A pipeline está **incompleta**. Os steps de segurança precisam ser implementados por você.

## Sua missão
1. Implementar os steps de segurança no `pipeline.yml`
2. Fazer a pipeline **quebrar** ao detectar os problemas
3. Corrigir as vulnerabilidades encontradas
4. Fazer a pipeline **passar** com tudo verde ✅
5. Documentar o funcionamento da pipeline neste README

## O que implementar
- [ ] Secrets Scanning com **Gitleaks**
- [ ] SAST com **Semgrep**
- [ ] SCA com **Grype**
- [ ] Assinatura do artefato com cosign
- [ ] Deploy com **GitHub Pages**

## Como a pipeline funciona
> **Substitua este bloco pela sua explicação após implementar a pipeline.**
> Descreva cada step, o que ele faz e por que ele é importante para a segurança.
Iniciei o projeto dando um fork no repositório original. isso cria um repositório igual ao original, para que possamos trabalhar sem mexer no processo que está em produção.
Após isso, criei 2 branches, a main, e outra com nome teste, para não commitar direto na main branch.
Habilitado o GitHub Pages no repositório.
Implementado o Gitleaks (secrets scanning). Importante para detectar secrets no código. ex chaves e senhas
Removida as linhas com os findings, que eram keys hardcoded não utilizadas no arquivo script.js
Implementado o Semgrep (gate SAST). importante para detectar vulnerabilidades no código
Corrigido os findings do Semgrep
Instalado o Grype - gate SCA. importante para detectar bibliotecas desatualizadas (vulneráveis)
Atualizada as versões das libs barradas no gate SCA
Atualizada versão do git actions para 4.1.3
## URL de Produção
https://tozzimarcelo.github.io/projeto-devsecop-desafio/
