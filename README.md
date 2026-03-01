# Bedrock Teleport Holder Behavior Pack

This behavior pack adds a custom item that teleports you to fixed coordinates while held.

## Item
- Identifier: `bedrockmod:warp_relic`
- Intended acquisition: command-only with `/give` (hidden from creative inventory)
- Teleport destination while held: `8000 75 8000`

No recipe or loot integration is provided, so players only receive it via commands.

## Give command
```mcfunction
/give @s bedrockmod:warp_relic
```

## Files
- `manifest.json` — behavior pack metadata.
- `items/warp_relic.json` — custom item definition.
- `functions/tick.json` — registers the tick function.
- `functions/tick.mcfunction` — teleports players holding the item.
