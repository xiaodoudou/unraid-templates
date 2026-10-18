# unraid-templates

Unraid Docker templates, one folder per app:

| Template | App |
|---|---|
| [homelabdash](homelabdash/homelabdash.xml) | [homelabdash](https://github.com/xiaodoudou/homelabdash), a homelab dashboard configured in one YAML file |
| [PlexIPTV](PlexIPTV/PlexIPTV.xml) | [PlexIPTV](https://github.com/xiaodoudou/PlexIPTV), an IPTV subscription as live TV in Plex, by pretending to be an HDHomeRun tuner |
| [SyncYomi](SyncYomi/SyncYomi.xml) | [SyncYomi](https://github.com/SyncYomi/SyncYomi), a self-hosted server that syncs your manga library and reading progress between TachiyomiSY and Komikku devices |

## Installing one

Search for the app in the Apps tab (Community Applications).

If it isn't listed there, load the template by hand from the Unraid terminal, for example for homelabdash:

```sh
curl -fsSL -o /boot/config/plugins/dockerMan/templates-user/my-homelabdash.xml \
  https://raw.githubusercontent.com/xiaodoudou/unraid-templates/main/homelabdash/homelabdash.xml
```

Then go to Docker, Add Container, and pick homelabdash under Template.

## Problems

Problems with an app go to its project's issues. Problems with a template itself, such as a wrong path or a missing setting, can be reported [here](https://github.com/xiaodoudou/unraid-templates/issues).

`ca_profile.xml` is the profile Community Applications shows for this repository.
