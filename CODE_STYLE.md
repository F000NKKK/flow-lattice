# Code style and architecture

Flow Lattice is a bootstrap placeholder. It has no implemented policy
compiler or accepted crate architecture. The following are design guidelines
derived from the existing Lattice repositories, not implemented contracts.

- Keep policy parsing and validation, deterministic compilation and plan
  execution separate. The intended output is a platform-neutral plan; OS
  mutation belongs to an integration layer, not the compiler itself.
- Define typed rules, errors, precedence, conflict behavior and explicit
  unsupported cases before committing to a public API. Cover equivalent and
  conflicting rules with deterministic tests.
- Use small testable interfaces at integration boundaries, explicit capability
  checks where platform execution is involved, and no hidden OS side effects.
- Follow Rust formatting, public rustdoc, meaningful examples and tests, and
  the workspace CI gates. Record design decisions in ADRs as required by the
  repository workflow.

The relationship to DNS routing hooks and net-lattice plans remains to be
designed and validated; these guidelines do not prescribe a dependency graph.
