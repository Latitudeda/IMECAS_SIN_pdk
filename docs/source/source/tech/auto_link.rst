auto_link.py
=============

Define the auto link policies between different waveguide type.

For example:

``(type(WG.Channel.C.WIRE) >> type(WG.Channel.C.WIRE), LinkPrefer(WG.Channel.C.WIRE), BendUsing(WG.Channel.C.WIRE.BEND))``

It means that when the start and end waveguide are both ``WG.Channel.C.WIRE``, the automated waveguide type for routing will be ``WG.Channel.C.WIRE`` and an automated bend ``WG.Channel.C.WIRE.BEND`` will be added at a 90 degree turn.


Users are allowed to define and set ``DEFAULT`` to their own specific linking policy.

