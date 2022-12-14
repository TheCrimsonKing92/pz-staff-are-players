# Staff Are Players

In vanilla, the Project Zomboid (PZ) load process sets active any basic power (god mode, ghost mode, invisibility) to which the player's role has access. This has implications such as automatically healing a moderator player on login, which disrupts the normal course of play for those players.

Staff Are Players (SAP) solves this scenario by requiring manual assumption (via the newly added command /onduty) and surrender (via the newly added command /offduty) of staff powers. While the core PZ player loading logic cannot be altered via a Workshop-distributed mod, SAP sidesteps this by saving the current state of the player character at logout and going on duty; at both login and going off duty, role-based powers are disabled, and the previous state is re-applied to the character. Additionally, staff are automatically taken off duty on logout for consistency.
