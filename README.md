*Written by Claude Opus 5.5 (Claude Code, high effort) on behalf of GrimsVerk, who skimmed it. The research, the test-build code changes, the measurements and this text are Claude's work.*

# NVIDIA NR runtimes 310.8 vs 310.9.16

**View the report: https://grimsverk.github.io/nr-runtime-research/**

A research report on the DLSS-NR runtimes 310.8 and 310.9.16:

- **Static analysis** of both runtimes: models, presets and every NGX parameter, with addresses, file offsets and decompile line numbers ([static.html](https://grimsverk.github.io/nr-runtime-research/static.html)).
- **Every setting tested in The Witcher 3** on frozen photo-mode frames, with both runtimes switched live in the same frame.
- **All three model/runtime combinations** compared on looks and GPU cost: the new small model (310.9.16 default), the old model inside 310.9.16 (preset 1), and the old model in 310.8.
- **Model cost per working scale** and what a fixed cost in ms does to fps.
- **ControlMask:** a working implementation and how-to ([controlmask.html](https://grimsverk.github.io/nr-runtime-research/controlmask.html)).
- **Noisy-domain NR feasibility memo** ([noisy-domain.html](https://grimsverk.github.io/nr-runtime-research/noisy-domain.html)).

Measurements and pictures come from a research build of [GrimsVerk's OptiScaler-NR fork](https://github.com/GrimsVerk/OptiScaler-DLSSNR-PreSR-Multipass) (v0.3.8, commit ac313d06); its source changes are in `research-build-source.patch`.

The repository contains only HTML pages, JPEG screenshots and a source patch. No DLLs, executables, model weights or NVIDIA code.

To view offline: download the repository (Code > Download ZIP), extract it, and open `index.html`.

## License

MIT, see [LICENSE](LICENSE).
