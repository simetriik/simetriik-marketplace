# simetriik-marketplace

Catalogue **privé** des plugins Claude Code de Simetriik Solutions (marketplace `simetriik`).
Procédure complète : `../marketplace-privee-guide.md`.

| Plugin | Dépôt (privé) | Installation |
|---|---|---|
| simetriik-forge | `dxokal/simetriik-forge` | `claude plugin install simetriik-forge@simetriik` |
| simetriik-guilde | `simetriik/simetriik-guilde` | `claude plugin install simetriik-guilde@simetriik` |
| axice | `simetriik/axice` | `claude plugin install axice@simetriik` |

## Installer sur une machine
```bash
claude plugin marketplace add simetriik/simetriik-marketplace
claude plugin install simetriik-forge@simetriik
claude plugin install axice@simetriik
claude plugin install simetriik-guilde@simetriik
```
L'accès suit les droits GitHub de la machine (clé SSH ou `gh auth setup-git`).

## Points à régler pour axice (dépôt simetriik/axice)
- Le dépôt est **public** : pour une marketplace entièrement privée, le passer en privé (`gh repo edit simetriik/axice --visibility private --accept-visibility-change-consequences`).
- Il contient encore son propre catalogue `.claude-plugin/marketplace.json` (marketplace `alolo-marketplace`) : le supprimer dans ce dépôt pour n'avoir que ce catalogue central.

## Publier une mise à jour d'un plugin
Augmenter `version` dans le `plugin.json` du plugin, pousser son dépôt ; ce catalogue ne change pas.
