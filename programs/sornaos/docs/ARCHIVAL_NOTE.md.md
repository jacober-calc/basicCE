# ARCHIVAL NOTE

## Regarding the Sorna Field Terminal Reconstruction

This document was written to accompany the reconstructed firmware
environment now running on TI-84 Plus CE hardware. It is intended to
explain, in plain technical narrative, how the original device was
recovered, how it moved through corporate custody, and how it ultimately
became executable in its present form. The account is based on hardware
inspection, asset records, auction documentation, and subsequent
reverse-engineering work performed by the individual responsible for the
current reconstruction.

------------------------------------------------------------------------

The field terminal was recovered from Isla Sorna sometime in late 1996
or early 1997, during the final phase of corporate asset retrieval
conducted after InGen's operational collapse. By that time the island
had been partially reclaimed by vegetation, and only limited salvage
teams were authorized to extract equipment that could be inventoried,
litigated, or liquidated. The device in question was discovered in a
damaged veterinary storage area, likely left behind during the 1995
hurricane evacuation that precipitated Site B's permanent abandonment.

Its location is instructive. It was not found in an executive office or
central control suite, but in a staging area adjacent to field
operations. That placement suggests the device was actively in
circulation at the time of evacuation --- not archived, not obsolete,
but part of daily operational use. It was a working terminal, not a
relic.

It was not cataloged as a proprietary computing unit. It was logged as a
"modified handheld instrumentation device." The casing resembled a TI-82
graphing calculator, and without power it was indistinguishable from
retail hardware. Its firmware was inaccessible at the time of recovery
due to battery corrosion and minor board damage. It was boxed with other
small electronics and transported off-island with no particular
significance attached to it.

During InGen's dissolution proceedings, multiple subsidiaries and asset
lots were acquired by outside entities. Among them was BioSyn, which
quietly acquired several lots of laboratory and computing equipment
through intermediary holding companies. BioSyn's interest in InGen's
intellectual property is well documented. However, this device did not
appear valuable at first inspection. It would not power on reliably, and
its modified ROM was unreadable without specialized tooling that, at the
time, BioSyn technicians either did not possess or did not prioritize.

The device was moved into long-term storage at a BioSyn warehouse
facility. It remained there for several years, effectively inert. The
damage sustained during the storm and subsequent neglect made it
unreliable on its native hardware. The battery contacts were unstable,
and internal memory addressing behaved unpredictably when power was
applied. It is likely that engineers attempted to assess it briefly,
determined that it was neither a data repository nor a server node, and
deemed it low priority.

Had it functioned normally, they might have recognized its significance.
The firmware reveals a facility that was not chaotic in its final days,
but structured. The menu hierarchy is orderly. The modules are
compartmentalized. Population counts are reconciled against expected
baselines. Vital signs are evaluated using statistical deviation.
Construction is tracked. Document control is enforced. Ethics committees
are meeting. Transfer protocols are being updated. Even hurricane
preparation follows formal escalation levels.

This was not a failing system in disarray. It was an organization still
attempting to operate within procedure.

BioSyn's own corporate instability in the early 2000s led to
consolidation and liquidation of nonessential holdings. As divisions
were dissolved and research priorities shifted, archived equipment was
cleared in batches. The Sorna terminal passed quietly into a secondary
liquidation channel. It did not move through scientific auction houses
or specialty resellers. Instead, it entered general surplus inventory
and disappeared into the broad ecosystem of online resale markets.

In 2017, it surfaced on eBay.

The listing was unremarkable: "Vintage TI Calculator -- For Parts or
Repair." The photographs were grainy. The casing showed minor
discoloration and a small adhesive label on the rear panel reading "DO
NOT REMOVE DEVICE." That label caught the attention of a calculator
enthusiast browsing surplus electronics. Members of communities like
Cemetech tend to notice such things. The buyer did not recognize its
origin, but he recognized that it was not standard retail firmware.

The device arrived nonfunctional. The screen flickered but did not
complete boot. Standard TI key combinations failed to access any known
OS routines. However, the enthusiast in question was not deterred by
damaged hardware. He was accustomed to extracting value from obsolete
devices. He stabilized the power rails, replaced corroded contacts, and
carefully accessed the ROM through hardware-level interfacing rather
than through normal user entry.

What he discovered was not a modified student calculator. It was a
locked firmware environment.

The ROM image did not contain the usual TI-82 operating system calls. It
contained structured menu branches, static message tables, and
references to modules labeled "Dinosaur Count," "Security Information,"
and "Network Initialization." The device had clearly functioned as a
thin client terminal. It attempted to connect outward to a host system
before enabling certain functions. Without that host, portions of the
system terminated locally.

More revealing than the code itself was what the structure implied about
Site B in 1995. The Dinosaur Count module presents reconciled figures
--- expected versus actual --- suggesting that population modeling was
not theoretical but active. The numbers align. There is no drift. The
Status module references σx, indicating monitored deviation within
species cohorts. That level of statistical framing implies daily data
collection and centralized processing. The Tracking module organizes
coordinates within bounded control areas, not free wilderness. The
language throughout assumes perimeter, zoning, containment.

The device represents a moment before systems failed. It captures Site B
in its procedural phase --- structured, measured, networked --- rather
than in its feral aftermath.

The problem was that the original TI-82 hardware could not meaningfully
run its own recovered image in stable form. Memory constraints,
addressing irregularities caused by board damage, and the inherent
limitations of the early 1990s architecture prevented reliable
exploration. The enthusiast could read the ROM but not execute it fully.

The breakthrough came not from repairing the old device but from
abandoning it.

The TI-84 Plus CE, released decades later, offered sufficient memory
capacity, display resolution, and processing stability to replicate the
interface environment in software. While not architecturally identical,
it shared enough lineage with the TI-82 platform to allow structural
reconstruction. The screen dimensions were compatible. The menu system
could be reproduced. The CE's RAM allowed the entire firmware shell to
exist without truncation.

The enthusiast manually rebuilt the interface logic in TI-BASIC,
recreating every branch, every static message, and even the failed
network handshake routine. Randomized values were introduced where the
original firmware clearly expected live telemetry from island sensors.
The goal was not to modernize the system, but to reconstruct its
behavior faithfully within the constraints of a contemporary TI
environment.

When the reconstructed program finally executed cleanly on the TI-84
Plus CE, it behaved as the original likely had on Isla Sorna between
1993 and 1995. It booted to a corporate splash screen. It navigated
through hierarchical menus. It displayed reconciled population counts
and statistical deviation markers. It attempted to connect to a host
server that no longer exists and returned quietly to its main menu.

The hardware that once relied on a living network had found new life in
emulation.

For calculator enthusiasts, the achievement lies in the elegance of the
port. A firmware shell once locked to proprietary silicon now runs
smoothly on descendant hardware available at retail. The architecture
has evolved, but the logic remains intact.

For those who recognize the corporate names embedded in the strings, the
significance is more unsettling. The interface is not theatrical. It is
administrative. It reflects a facility that attempted to quantify and
manage biological systems through structured menus and statistical
baselines.

The terminal was never designed to operate independently. It was a node
in a distributed attempt to impose order.

That system collapsed.

The node survived.

It now runs, paradoxically, on hardware descended from the very platform
it once used --- not as an instrument of control, but as a preserved
artifact of a network that failed.

And each time the user selects "Current Assignment" and watches the
connection attempt fail, the program demonstrates its own history more
accurately than any dramatic reconstruction could.

The server is gone.

The menu remains.
