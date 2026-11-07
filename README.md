# J-Express plugin for ChatGPT

J-Express is a browser-based application for exploring and analyzing numeric matrices: gene expression, bulk and single-cell RNA-seq, proteomics and text embeddings. This repository holds the ChatGPT plugin package: the portable manifest (`plugin.json`), the J-Express MCP server (`mcp.json`), five scientific analysis skills, logos, and the submission and verification notes in [chatgpt/](chatgpt/).

The Claude plugin, with the same MCP server and skills, lives in [resonalis/jexpress-plugin](https://github.com/resonalis/jexpress-plugin). The two are kept apart because the Claude plugin directory refuses scripts and SVG files in a plugin folder.

## Validate and package

The [Validate ChatGPT plugin package](.github/workflows/validate-chatgpt-plugin.yml) workflow checks `plugin.json` and `mcp.json` against the Agent Plugins 1.0.0 schemas, runs [scripts/validate_plugin.py](scripts/validate_plugin.py), and uploads `jexpress-chatgpt-plugin.zip` as a build artifact. To run the checks locally:

```bash
python -m pip install jsonschema==4.25.1 PyYAML==6.0.3
python scripts/validate_plugin.py
```

## Privacy and support

See [PRIVACY.md](PRIVACY.md) and https://resonalis.com/privacy/. Contact: contact@resonalis.com.

## License

Apache-2.0. See [LICENSE](LICENSE).
