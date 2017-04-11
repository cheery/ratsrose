# Stack reservation and allocation to allow spilling

Rather than implicitly reserving the location for register spilling, I'd prefer if it came from a code object that can do the reservation explicitly.

The spilling is allowed to fail if there is no reservation for spilled registers.
