# Meu Pacote Funcoes

Pacote Python interno com funcoes uteis para a equipe.

## Estrutura

```text
meu-pacote-funcoes/
├─ pyproject.toml
├─ README.md
├─ .gitignore
└─ meu_pacote_funcoes/
   ├─ __init__.py
   └─ funcoes.py
```

## Instalar localmente para teste

Dentro da pasta do projeto:

```bash
pip install -e .
```

## Uso

```python
from meu_pacote_funcoes import soma, saudacao

print(soma(2, 3))
print(saudacao("Joao"))
```

## Subir para o GitHub

```bash
git init
git add .
git commit -m "Primeira versao do pacote"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/meu-pacote-funcoes.git
git push -u origin main
```

Substitua `SEU_USUARIO` pelo seu usuario ou organizacao do GitHub.

## Instalar pelo GitHub

```bash
pip install git+https://github.com/SEU_USUARIO/meu-pacote-funcoes.git
```

## Instalar branch especifica

```bash
pip install git+https://github.com/SEU_USUARIO/meu-pacote-funcoes.git@develop
```

## Instalar tag especifica

Crie a tag:

```bash
git tag v0.1.0
git push origin v0.1.0
```

Instale a tag:

```bash
pip install git+https://github.com/SEU_USUARIO/meu-pacote-funcoes.git@v0.1.0
```

## Atualizar pacote

Altere a versao no `pyproject.toml`, por exemplo:

```toml
version = "0.2.0"
```

Depois:

```bash
git add .
git commit -m "Atualiza funcoes do pacote"
git tag v0.2.0
git push
git push origin v0.2.0
```

Os colegas atualizam com:

```bash
pip install --upgrade git+https://github.com/SEU_USUARIO/meu-pacote-funcoes.git@v0.2.0
```
