# 📘 Guia de Comandos Git

Este arquivo contém um resumo útil de comandos Git com explicações rápidas. Ideal para consulta no dia a dia de desenvolvimento.

---

## 🔍 Status do Repositório

```bash
git status
```
Exibe o estado atual dos arquivos no repositório (modificados, staged, untracked, etc).

```bash
git status --short
```
Mostra uma versão resumida do status, útil para visualização rápida:
- `??` → Arquivos não rastreados (untracked)
- `A`  → Arquivos adicionados ao stage
- `M`  → Arquivos modificados
- `D`  → Arquivos deletados

---

## ➕ Adicionar Arquivos

```bash
git add <arquivo>
```
Adiciona um arquivo específico ao stage.

```bash
git add --all
git add -A
git add .
```
Adiciona todas as mudanças (novos arquivos, modificações e deleções) ao stage.

---

## ✅ Realizar Commit

```bash
git commit -m "mensagem"
```
Cria um commit com a mensagem fornecida.

```bash
git commit -a -m "mensagem"
```
Adiciona automaticamente todos os arquivos modificados já rastreados e cria o commit.

---

## 📜 Histórico de Commits

```bash
git log
```
Mostra o histórico de commits do repositório local.

```bash
git log origin/master
```
Mostra o histórico de commits da branch `origin/master`.

Navegação no `log`:
- `SHIFT + G` → Vai para o final
- `q` → Sai do log

---

## ❓ Ajuda

```bash
git command -help
```
Mostra a ajuda para um comando específico.

```bash
git help --all
```
Lista todos os comandos disponíveis no Git.

---

## 🌿 Gerenciar Branches

```bash
git branch
```
Lista as branches locais.

```bash
git branch -a
```
Lista todas as branches (locais e remotas).

```bash
git branch -r
```
Lista apenas as branches remotas.

```bash
git branch <nome-da-branch>
```
Cria uma nova branch.

```bash
git checkout <branch>
```
Muda para uma branch existente.

```bash
git checkout -b <branch>
```
Cria uma nova branch e já muda para ela.

---

## 🔀 Mesclar Branches

```bash
git merge <branch>
```
Mescla a branch especificada com a branch atual.

```bash
git merge origin/master
```
Mescla as mudanças da branch `origin/master` com a branch atual.

```bash
git branch -d emergency-fix
```
Deleta a branch `emergency-fix`.

---
