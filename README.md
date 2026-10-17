# simetriik-marketplace

Catalogue **privé** des plugins Claude Code de Simetriik Solutions (marketplace `simetriik`).
Procédure complète : `../marketplace-privee-guide.md`.

| Plugin | Dépôt (privé) | Installation |
|---|---|---|
| forge | `simetriik/forge` | `claude plugin install forge@simetriik` |
| guilde | `simetriik/guilde` | `claude plugin install guilde@simetriik` |
| axice | `simetriik/axice` | `claude plugin install axice@simetriik` |

## Installer sur une machine
```bash
claude plugin marketplace add simetriik/simetriik-marketplace
claude plugin install forge@simetriik
claude plugin install axice@simetriik
claude plugin install guilde@simetriik
```
L'accès suit les droits GitHub de la machine (clé SSH ou `gh auth setup-git`).

## Publier une mise à jour d'un plugin
Augmenter `version` dans le `plugin.json` du plugin, pousser son dépôt ; ce catalogue ne change pas.
