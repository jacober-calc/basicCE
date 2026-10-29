# SORNA_TERMINAL_CE Reconstruction Notes

### Author: \[handle redacted\]

------------------------------------------------------------------------

## Overview

This document describes the reconstruction of a recovered Sorna field
terminal firmware environment for the TI-84 Plus CE platform.

The original device was a heavily modified TI-82 unit operating with
custom ROM. Standard TI operating system functionality was removed or
suppressed. The familiar math interface did not exist. Instead, the
firmware implemented a structured, menu-driven operational shell
designed to interface with an external host network.

The recovered hardware no longer had access to its backend
infrastructure. However, the firmware image was largely intact. After
dumping the ROM and analyzing string tables and control flow, I rebuilt
the interface logic in TI-BASIC for the TI-84 Plus CE.

This is not an emulator.\
It is a functional reconstruction of the observed interface behavior.

------------------------------------------------------------------------

## Boot Sequence

Upon execution:

-   Screen clears.
-   Static corporate splash text is displayed.
-   Timed delay.
-   Screen clears again.
-   Control transfers to the primary hub.

There are no user interrupts at boot. This mirrors embedded firmware
behavior rather than typical TI program conventions.

------------------------------------------------------------------------

## Main Hub (Lbl A)

The program uses a central dispatcher label to manage state transitions.
All navigation routes back to this label or to a defined submenu parent.
There is no recursion or stack-based navigation.

Primary options:

-   Company Messages\
-   Current Assignment\
-   Dinosaur Count\
-   Dinosaur Status\
-   Dinosaur Tracking\
-   Incident Reporting\
-   Security Information\
-   Exit

Each selection branches using `Menu(` and `Goto` statements.

This design reflects constrained firmware architecture rather than
free-form calculator scripting.

------------------------------------------------------------------------

## Network Simulation Modules

Two modules simulate network handshake behavior:

### Current Assignment

### Incident Reporting

Both execute the same sequence:

-   Display: "Trying to connect..."
-   Timed delay
-   Display: "Could not connect!"
-   Return to main hub

These are not errors. They represent a client terminal attempting
authentication with a now-missing host infrastructure.

------------------------------------------------------------------------

## Data Modules

### Dinosaur Count

Displays static expected vs. actual population in `n/n` format.

Header includes `Σ/n`, implying statistical normalization or averaged
reconciliation.

Values are deterministic. This simulates reconciled hourly inventory
rather than live telemetry.

------------------------------------------------------------------------

### Dinosaur Status

Displays species-level deviation values using:

    round(rand,4)*10

This generates a 0--10 range with decimal precision.

Header displays `σx`, indicating deviation within species group.

Values regenerate each access, simulating live biological variance
metrics.

------------------------------------------------------------------------

### Dinosaur Tracking

Displays pseudo-coordinate pairs using:

    round(rand,2)*100

This yields integer-like values between 0--100.

Coordinates are displayed as x,y pairs per species.

Regeneration on each execution simulates dynamic movement within defined
control zones.

------------------------------------------------------------------------

## Company Messages

Implements a nested menu branch functioning as a static memo repository.

Each message:

-   Clears screen
-   Displays multi-line formatted output
-   Uses `Pause`
-   Returns to message hub

This behavior mirrors ROM-based bulletin access systems.

------------------------------------------------------------------------

## Security Module

Two sequential screens display:

1.  Data sensitivity and property warning\
2.  Compliance requirement referencing Document 112/4A

Each screen requires user acknowledgment via `Pause`.

Control then returns to the main hub.

------------------------------------------------------------------------

## Exit Routine

Shutdown sequence displays:

-   "SENSITIVE DATA"
-   Corporate copyright line
-   A small numeric identifier at lower right

Timed delay follows before program termination.

The numeric identifier is intentionally undocumented.

------------------------------------------------------------------------

## Conversion Rationale

The original TI-82 hardware lacked sufficient RAM and execution headroom
to meaningfully explore the recovered firmware image in reconstructed
form.

The TI-84 Plus CE provides:

-   Increased program memory
-   Faster execution
-   Stable display handling
-   Improved development tooling

The CE platform allows the reconstructed shell to operate without memory
truncation or execution instability.

------------------------------------------------------------------------

## Design Philosophy

This reconstruction preserves:

-   Hierarchical menu structure\
-   Deterministic navigation\
-   Embedded-style flow control\
-   Offline network failure behavior

There are no hidden inputs or undocumented key paths.

The structure is intentionally rigid.

It behaves less like a calculator program and more like a constrained
firmware shell --- because that is the architecture it was designed to
replicate.

If you are running this on a TI-84 Plus CE, you are executing a modern
recreation of a mid-90s embedded field terminal environment built on the
same architectural lineage.

That continuity is deliberate.
