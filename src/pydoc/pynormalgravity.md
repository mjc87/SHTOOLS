# NormalGravity()

Calculate the normal gravity on a flattened ellipsoid in geocentric coordinates using the formula of Somigliana.

# Usage

value = NormalGravity (geocentriclat, gm, omega, a, b)

# Returns

value : float, ndarray
:   The normal gravity in SI units.

# Parameters

geocentriclat: float, array_like
:   Geocentric latitude in degrees.

gm : float
:   The gravitational constant multiplied by the mass of the planet.

omega : float
:   The angular rotation rate of the planet.

a : float
:   The semi-major axis of the flattened ellipsoid on which the normal gravity is computed.

b : float
:   The semi-minor axis of the flattened ellipsoid on which the normal gravity is computed.

# Description

NormalGravity will calculate the magnitude of the predicted gravity (in m/s^2) on a flattened ellipsoid using Somigliana's formula. The latitude is input in geocentric coordinates in degrees, which is later converted to geodetic coordinates in the routine for use with Somigliana's formula. Other input parameters include gm, the product of the gravitational constant and the planet's mass, and the semi-major and semi-minor axes of the planet, a and b, respectively. For further details, see sections 2.7 and 2.8 of Physical Geodesy (Hofmann-Wellenhof and Moritz).

# References

Hofmann-Wellenhof B, and H. Moritz, "Physical Geodesy," second edition, Springer, Wien, 403 pp., 2006.
