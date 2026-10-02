# [MODEL] Implement basic stock-flow consistency checks

**Labels:** `good first issue`, `model`, `python`, `area:model`, `priority:starter`

## Goal

Create a minimal prototype that checks a few stock-flow accounting identities before the full economic engine exists.

## Suggested checks

- financial assets = corresponding financial liabilities across sectors;
- balance-sheet identity for each sector;
- opening stock + flows = closing stock;
- government deficit / surplus consistency;
- bank loans and deposits consistency in the toy system.

## Acceptance criteria

- Include unit tests with valid and intentionally invalid cases.
- Produce a clear error message when an identity fails.
- Keep the prototype independent from any specific game UI.
