# CursedDeck

Adds the **Cursed Deck** — every unambiguous downside from Balatro's base decks
on a single deck, with none of the upsides that normally pay for them.

- **-1 hand every round** — from Black Deck
- **-1 Joker slot** — from Painted Deck
- **-1 consumable slot** — from Nebula Deck
- **Earn no Interest** — from Green Deck
- **X2 base Blind size** — from Plasma Deck

Ten of the fifteen base decks have no downside at all. Of the remaining five,
each one hands you something to compensate — Black gives a Joker slot back,
Nebula gives a free Telescope voucher, Painted gives two extra cards in hand,
Green pays you per unused hand and discard, and Plasma balances your chips and
mult. The Cursed Deck takes the penalty from each and none of the compensation.

Abandoned and Erratic are deliberately left out. Removing face cards and
randomizing ranks are usually considered buffs, not downsides.

## Install

1. Install [Steamodded](https://github.com/Steamodded/smods) (1.0.0~BETA-0400a
   or newer).
2. Drop the `CursedDeck` folder into your `Mods` directory.
3. Launch the game. The Cursed Deck appears in deck select, unlocked.

No `lovely.toml` is required — this mod is a plain Steamodded deck declaration
and patches nothing.

## Compatibility

Do **not** run this alongside the NickTGMods pack, which bundles the same deck.
Both will load and you will get two Cursed Deck entries in deck select under
different keys.

Nothing here hooks or wraps a vanilla function, so conflicts with other mods are
unlikely.

## Notes

**Plasma's balancing does not apply.** In the base game, Plasma Deck doubles
blind sizes *and* balances your chips and mult. The balancing is keyed on the
literal deck name in `Back:trigger_effect`, while the doubled blind size flows
through a generic starting parameter. A differently named deck therefore
inherits the blind scaling without the balancing. This is intended: the point of
the deck is the penalty, not the trade.

**The deck back art is a placeholder.** It reuses the vanilla Challenge Deck
sprite. Swapping in custom art is a two-line change — see the header comment in
`CursedDeck.lua`.

## License

MIT. See [LICENSE](LICENSE).
