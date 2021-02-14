Most logic is in cargo/core/workspaces.rs
find_roots stops at the first root, should keep going recursively.
find_roots doesn't appear to search up if the current package is virtual/has a workspace?
find_members should keep going recursively down

validate should already be checking that every package believes it has the same root,
so this should be enough to make the feature work?