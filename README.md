# Nomads-Developement-Spikes
This Is A Simple standalone script that allows people to implement spikes for LEO. Comes with perms setup as well to allow only certain perms to use. This does work with players and AI 

Discription___________________________________________________
/spikes_clearall — nukes every spike on the map. ACE-protected.

Police-only (or any group) restriction — toggle with Config.RequireAceUse = true. Uses ACE cprp_spikes.use.

Auto-cleanup on player drop — their spikes are removed when they disconnect.

---Still standalone. No ESX/QBCore. All ASCII-safe.-----

Quick setup
drop into resources in your server files.

*In Server.cfg*
ensure cprp_spikes in server.cfg

Optional ACE gating you can add:

add_ace group.police cprp_spikes.use allow
add_ace group.admin  cprp_spikes.admin allow
add_principal identifier.steam:110000112345678 group.police


Then set Config.RequireAceUse = true in config.lua.

Usage-----------------------------------------------------------------

Default keybinds (rebindable in Settings → Key Bindings → FiveM):

F6: 1 strip

F7: 2 strips

F8: 3 strips

F9: pickup nearest

Chat aliases: /spike1, /spike2, /spike3, /spikepickup

Admin: /spikes_clearall
