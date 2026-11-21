# VeilCore archive

A public copy of every batch VeilCore has dated, kept outside VeilCore.

Every six hours a GitHub Action copies each batch from the registry into `data/` and checks it without any VeilCore server: the batch root, its Bitcoin stamp and its RFC 3161 timestamp. Whatever changed is committed, so this repository's history is a dated, public record of what the registry served and when. If the registry ever changed an earlier answer, both versions are kept here and the run fails.

The scripts live in [veilcore-api](https://github.com/hunterincoming/veilcore-api/tree/main/scripts/mirror). To run your own copy, see [docs/run-a-witness.md](https://github.com/hunterincoming/veilcore-api/blob/main/docs/run-a-witness.md).

## License

Everything in this repository, the mirrored data in `data/` and the workflow that fetches it,
is dedicated to the public domain under [CC0 1.0](LICENSE). The mirror scripts the workflow
runs are in veilcore-api, under that repository's license.
