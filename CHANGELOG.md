
1.0.0-beta7 (Dan Reynolds)

- Fix issue where read policies were attempted to be evaluated for non-normalized entities not yet in the cache if they had a different store field name with the same name
  already written in the cache.

1.0.0-beta6 (Dan Reynolds)

- Adds a `storage` dictionary by unique `storeFieldName` for queries or `ID` for normalized entities in the policy action object so that arbitrary meta information can be stored across multiple policy action invocations.

1.0.0-beta5 (Dan Reynolds)

- Adds support for a `renewalPolicy` type and global config option for specifying how type TTLs should be renewed on write vs access
- Adds the `expire` API for evicting all entities that have expired in the cache based on their type's or the global TTL.

1.0.0-beta4 (Dan Reynolds)

- [BREAKING CHANGE] Adds support for a default TTL option that applies to all types

1.0.0-beta3 (Dan Reynolds)

- Ensure that empty field arguments are still passed as an empty object as the variables in the policy event.

1.0.0-beta2 (Dan Reynolds)

- Bumps to latest Apollo version (3.1)
- Adds audit logging for better entity debugging through the type map and invalidation policy manager

1.0.0-beta1 (Dan Reynolds)

- Initial beta release 🚀