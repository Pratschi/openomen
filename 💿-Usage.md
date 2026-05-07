# OpenOMEN Usage

To see OpenOMEN's help and information, run `openomen --help`, but just `openomen` is also valid.

## See System Information
Use it to report your system Specs and Information when reporting an issue on GitHub or Discord.

```bash
openomen info
```

## Updating OpenOMEN
Use this command to automatically update OpenOMEN to the latest available version.
```bash
openomen update
```

## Manage and See Fans Status
These commands are available to manage your fan modes and see their status.

```bash
openomen fan status     # Show current fan status
openomen fan auto       # Set fans to Auto/BIOS control
openomen fan max        # Set fans to maximum RPM
openomen fan toggle     # Toggle fans max mode on/off
```


## See System Stats
These commands are available, and all of them are compatible with the `-w` or `--watch` argument, to make its stats update in real time every 2 seconds.

```bash
openomen cpu       # See CPU info
openomen gpu       # See GPU info
openomen stats     # See combined CPU, GPU, Power and Fan Info
```

## Manage and See Power Modes
These commands are available to manage your ACPI and Combined Power modes.

```bash
openomen status     # Show current power profile
openomen set        # Set an ACPI power profile directly
openomen apply      # Apply a combined profile (gaming, balanced, quiet)
openomen list       # List available profiles
```