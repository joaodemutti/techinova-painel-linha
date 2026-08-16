# Respostas do LAB 01

Nome: João Facin Demutti
Matricula:
Dupla (M2 em diante): Beatriz Campanha Silva

---

## M2 - Quem quebrou o painel

**Hash curto do commit que introduziu o erro:** 01ef93bf

**Autor:** Tarcisio Melo

**Data:** 2026-06-15 22:38:00 -0300 10

**Linha alterada (antes e depois):**

```
antes: return (leitura - 32) * 5 / 9;
depois: return leitura * 9 / 5 + 32;
```

---

## M3 - O segredo vazado

**O que voce esperava ver no `git status` e o que apareceu:**

Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

**Depois do push, alguem que clonar o repositorio ainda consegue ler a chave?
Responda em duas linhas, explicando o motivo:**

Sim, pois, fica tudo registrado no histórico do repositório possibilitando recuperar o valor e mudanças anteriores.
---

## M4 - Colisao

**O que significavam os marcadores que apareceram dentro do arquivo:**

- `<<<<<<<` : Início do bloco de conflito e estado atual da branch
- `=======` : Divisão entre o estado atual e as mudanças trazidas pelo merge
- `>>>>>>>` : Fim do bloco de conflito e mudanças trazidas pelo merge

**Qual pedaco veio de quem, e qual titulo voces decidiram manter:**

Depende do contexto do merge, no nosso caso a base foi a main então as mudanças conflitantes vieram do painel-b que foi mesclado posteriormente ao painel-a. Mantivemos o B, porém, poderiamos ter mesclado e mantido a mudança de ambas as branches.

---

## Casa - Incidente na linha 3

**Hash do commit que quebrou o painel:**

**Hash do commit de revert:**

**Por que `git revert` e nao `git reset` neste caso:**
