# webpack-util-logger

## Overview
Repo for designing / creating a logging utility for webpack, per this issue [discussion](https://github.com/webpack/webpack-cli/issues/87).

> Make a logger module for webpack instead of manually configuring this. ( Useful for both the CLI and webpack itself )


## Additional feedback / direction provided
1. > [@bebraw](https://github.com/webpack/webpack-cli/issues/87#issuecomment-319025814) - Not really. The logger module is something you should discuss on webpack core. Propose an API for that. The rest seem isolated to the CLI.

1. > @sokra We have `emitWarning` `emitError` for loaders and `compilation.warnings` `compilation.errors` for plugins, but the info/log counterparts are missing.  A better way for warnings/errors for plugins would be also great

1. > @TheLarkInn I think also you should consider the way's that Stats.js is used to produce final build information.