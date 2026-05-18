# amlmarketplaces/cohere

Claude Code marketplace federating all `@amlplugins/cohere-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-cohere": {
      "source": { "source": "github", "repo": "amlmarketplaces/cohere" }
    }
  },
  "enabledPlugins": {
      "cohere-chat@aml-cohere": true,
      "cohere-classify@aml-cohere": true,
      "cohere-datasets@aml-cohere": true,
      "cohere-embeddings@aml-cohere": true,
      "cohere-fine-tuning@aml-cohere": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/cohere`, cached under `~/.claude/plugins/cache/aml-cohere/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (6 total)

- `cohere-chat` — [@amlplugins/cohere-chat](https://github.com/amlplugins/cohere-chat)
- `cohere-classify` — [@amlplugins/cohere-classify](https://github.com/amlplugins/cohere-classify)
- `cohere-datasets` — [@amlplugins/cohere-datasets](https://github.com/amlplugins/cohere-datasets)
- `cohere-embeddings` — [@amlplugins/cohere-embeddings](https://github.com/amlplugins/cohere-embeddings)
- `cohere-fine-tuning` — [@amlplugins/cohere-fine-tuning](https://github.com/amlplugins/cohere-fine-tuning)
- `cohere-rerank` — [@amlplugins/cohere-rerank](https://github.com/amlplugins/cohere-rerank)

## Related

- npm packages: `@amlplugins/cohere-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
