# PlSchmidt_d1()

Compute all the Schmidt-normalized Legendre polynomials and first derivatives.

# Usage

p, dp = PlSchmidt_d1 (lmax, z)

# Returns

p : float, dimension (lmax+1)
:   An array of Schmidt-normalized Legendre polynomials up to degree lmax. Degree l corresponds to array index l.

dp : float, dimension (lmax+1)
:   An array of the first derivatives of the Schmidt-normalized Legendre polynomials up to degree lmax. Degree l corresponds to array index l.

# Parameters

lmax :integer
:   The maximum degree of the Legendre polynomials to be computed.

z : float
:   The argument of the Legendre polynomial.

# Description

PlSchmidt_d1 will calculate all of the Schmidt-normalized Legendre polynomials and first derivatives up to degree lmax for a given argument. These are calculated using a standard three-term recursion formula, and the integral of the Schmidt-normalized Legendre polynomials over the interval [-1, 1] is 2/(2l+1). Note that the derivative of the Legendre polynomials is calculated with respect to its arguement z, and not latitude or colatitude. If z=cos(theta), where theta is the colatitude, then it is only necessary to multiply dp by -sin(theta) to obtain the derivative with respect to theta.
