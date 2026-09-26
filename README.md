# Street Excavation Coordination

Dig once: a service that lets a city open a street once for all the underground work it needs, and then leave it alone.

Today the same street is often dug up several times within a few years, because water, district heating, electricity, telecom and other network operators plan their work separately. This project coordinates those plans so that overlapping works are combined into one joint excavation, every affected party and resident is notified, and the restored street is protected by a moratorium afterwards.

The pilot is the Töölö district of Helsinki, Finland. The service extends Helsinki's existing street-works system [Haitaton](https://haitaton.hel.fi) and uses national sources such as Traficom's Verkkotietopiste and Johtotieto.

## Status

Product definition. The full requirements are in **[PRD.md](PRD.md)**:

- Helsinki context and existing systems
- Goals, non-goals and success metrics
- Stakeholders, dig-once lifecycle and key user flows
- Functional requirements (FR-1 to FR-24), data model and integrations
- Policy rules, moratoriums and the public operator cooperation scorecard
- Non-functional requirements, phasing, risks and open questions

## Development environment

The repository includes a VS Code Dev Container (`.devcontainer/`) with Claude Code and Mistral Vibe preinstalled, based on Sitra's [agenttisen-ohjelmoinnin-kontti](https://github.com/sitrafund/agenttisen-ohjelmoinnin-kontti) template.

Requirements: [Docker Desktop](https://www.docker.com), [VS Code](https://code.visualstudio.com) and the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension.

```bash
git clone https://github.com/Jussi-Hermunen/street-excavation-coordination.git
cd street-excavation-coordination
code .
```

VS Code offers **Reopen in Container**; accept it and wait for the container to build. Then run `claude` or `vibe` in the terminal. If sign-in fails in the VS Code terminal, run `docker exec -it <container-name> bash` from your own terminal and sign in there once.
