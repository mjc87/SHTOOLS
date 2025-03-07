---
title: PlBar()
keywords: spherical harmonics software package, spherical harmonic transform, legendre functions, multitaper spectral analysis, Python, gravity, magnetic field
sidebar: mydoc_sidebar
permalink: pyplbar.html
summary:
tags: [python]
toc: false
editdoc: pydoc
---

Compute all the 4-pi (geodesy) normalized Legendre polynomials.

## Usage

p = PlBar (lmax, z)

## Returns

p : float, dimension (lmax+1)
:   An array of 4-pi (geodesy) normalized Legendre polynomials up to degree lmax. Degree l corresponds to array index l.

## Parameters

lmax : integer
:   The maximum degree of the Legendre polynomials to be computed.

z : float
:   The argument of the Legendre polynomial.

## Description

PlBar will calculate all of the 4-pi (geodesy) normalized Legendre polynomials up to degree lmax for a given argument. These are calculated using a standard three-term recursion formula. The integral of the geodesy-normalized Legendre polynomials over the interval [-1, 1] is 2.
