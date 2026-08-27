# thule

A micro-VM sandbox for [e](https://github.com/intuitumxyz/e): routes an
agent's tool execution — file reads/writes and shell commands — into an
isolated guest, with the workspace mounted through and the host (and its
credentials) never entering the guest.

> [!NOTE]
> This repository is a scaffold only. Nothing is implemented yet — see
> [CONTRIBUTING.md](CONTRIBUTING.md) for where things stand.

## Why

e has no built-in permission system by design — it runs with the
permissions of the process that launches it (see e's own
[`docs/sandboxing.md`](https://github.com/intuitumxyz/e/blob/main/docs/sandboxing.md)).
That's deliberate: the harness stays small, and isolation is left to
whatever wraps it. thule is that wrapper for the case where a container or
a restricted user isn't isolation enough — a full micro-VM boundary around
everything the agent's tools touch, integrated as an e extension rather
than folded into e itself.

## License

[MIT](LICENSE)
