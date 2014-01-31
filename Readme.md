# Speakeasy

This package provides cross-platform Go (#golang) helpers for taking user input
from the terminal while not echoing the input back (similar to `getpasswd`). The
package uses syscalls to avoid any dependence on cgo, and is therefore
compatible with cross-compiling.

The code herein was not written by me, but was compiled from two separate open
source packages. Unix portions were imported from [gopass][gopass], while
Windows portions were imported from the [CloudFoundry Go CLI][cf-cli]'s
[Windows terminal helpers][cf-ui-windows].

The [license for the windows portion](./LICENSE_WINDOWS) has been copied exactly
from the source (though I attempted to fill in the correct owner in the
boilerplate copyright notice).

[cf-cli]: https://github.com/cloudfoundry/cli "CloudFoundry Go CLI"
[cf-ui-windows]: https://github.com/cloudfoundry/cli/blob/master/src/cf/terminal/ui_windows.go "CloudFoundry Go CLI Windows input helpers"
[gopass]: https://code.google.com/p/gopass "gopass"
