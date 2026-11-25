# simetriik-marketplace

Catalogue **privé** des plugins Claude Code de Simetriik Solutions (marketplace `simetriik`).
Procédure complète : `../marketplace-privee-guide.md`.

| Plugin | Dépôt (privé) | Installation |
|---|---|---|
| forge | `simetriik/forge` | `claude plugin install forge@simetriik` |
| simetriik-guilde | `simetriik/simetriik-guilde` | `claude plugin install simetriik-guilde@simetriik` |
| axice | `simetriik/axice` | `claude plugin install axice@simetriik` |
| tunnu | `simetriik/tunnu` | `claude plugin install tunnu@simetriik` |

## Installer sur une machine
```bash
claude plugin marketplace add simetriik/simetriik-marketplace
claude plugin install forge@simetriik
claude plugin install axice@simetriik
claude plugin install simetriik-guilde@simetriik
claude plugin install tunnu@simetriik
```
L'accès suit les droits GitHub de la machine (clé SSH ou `gh auth setup-git`).

## Publier une mise à jour d'un plugin
Augmenter `version` dans le `plugin.json` du plugin, pousser son dépôt ; ce catalogue ne change pas.

## Migration depuis `simetriik-forge`
Le plugin s'appelle `forge`. Sur une machine qui avait l'ancien nom : `claude plugin uninstall simetriik-forge@simetriik`, `claude plugin marketplace update simetriik`, `claude plugin install forge@simetriik`, puis remplacer `simetriik-forge@simetriik` par `forge@simetriik` dans `enabledPlugins` des fichiers `settings.json`.
