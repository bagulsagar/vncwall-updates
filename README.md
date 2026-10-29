# VNC Wall Updates

This public repository is reserved for release assets and update metadata for VNC Wall desktop applications.

## Applications

- **VNC Wall Console** — update channel: `console`
- **VNC Wall Client Agent** — update channel: `agent`

Both applications use a shared release version/tag so a single GitHub Release can carry each application's installer and its own channel metadata (`console.yml` and `agent.yml`). The packaged applications must be configured with the matching channel and this repository as their GitHub update provider.

## Publishing notes

- Do not commit source code, access tokens, signing keys, or secrets here.
- Release assets are public and downloadable by anyone.
- Each release should include both apps' generated update manifests and the matching installers/blockmaps before rollout is considered complete.
- Use a new higher version for each release; do not overwrite an already-shipped version.

The updater feeds are not considered live until the Console and Client Agent package configurations are set and a release containing their assets and channel manifests has been published.