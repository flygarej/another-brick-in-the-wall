
# Project-State.md

## Scope

State of this TECO / TECO EMACS research project immediately before the
collaboration protocol was adopted in this chat.

---

# Verified Conclusions

## Research methodology

- Primary experimental targets are TECOC and TECO-64.
- TOPS-20 TECO is primarily a historical reference implementation.
- Original TECO EMACS is used when investigating architecture rather than
  later Standard TECO behaviour.
- Small discriminating experiments have repeatedly produced better progress
  than broad speculation.

## Search model

### Observation
- The search string is remembered after a successful search.
- Null searches reuse that remembered search string.
- Searches begin at the current dot.
- No evidence has been found for an additional hidden "continue previous match"
  search state.

### Working model
Search state currently consists of a remembered search pattern rather than an
implicit iterator over previous matches.

Status: Supported by experiments, still open to revision.

## Dialect understanding

Accepted model:

- TOPS-20 TECO represents an older and substantially smaller dialect.
- TECOC and TECO-64 are closer to later Standard TECO.
- Behavioural differences should initially be treated as dialect or historical
  evolution rather than implementation bugs.

## EMACS architecture

Verified/accepted:

- EMACS extends TECO using MIDAS code rather than only TECO macros.
- Long command names are resolved through the M.M mechanism.
- Q-register M provides historical compatibility with the older MM interface.
- Q-register ..Q contains a large command/variable dispatch structure.
- EMACS therefore introduces a higher-level command language layered on top of
  ordinary TECO.

## Active Questions

- What runtime objects make up EMACS command dispatch?
- Which parts of searching belong to the parser versus runtime state?
- Which observed behaviours are implementation-specific rather than language
  semantics?

## Next Recommended Experiments

1. Continue modelling runtime state rather than individual commands.
2. Investigate search/runtime objects.
3. Use TOPS-20 only when historical behaviour needs confirmation.
