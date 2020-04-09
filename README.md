COEFF(1) - General Commands Manual

# NAME

**coeff** - compare sensor and certificate coefficients

# SYNOPSIS

**coeff**
\[*directory*]

# DESCRIPTION

The
**coeff**
utility differentially compares sensor coefficients between
calibration certficates and instrument log captures.

The mounted ISO9660 or FAT filesystem, or optional
*directory*,
is recursively searched for sensor coefficients,
and all values found are compared.
Only one ISO9660 or FAT filesystem may be mounted at a time.

# FILES

*/usr/local/share/coeff/coeff.lst*

> Sorted list of record value pairs from NetSuite.

# EXIT STATUS

The **coeff** utility exits&#160;0 on success, and&#160;&gt;0 if an error occurs.

# SEE ALSO

sort(1),
mount(8)

# AUTHORS

**coeff**
was written by
Chris Hettrick &lt;chris@structfoo.com&gt;.

# CAVEATS

Tested only on Xchange series instruments and sensors.

The file
*/usr/local/share/coeff/coeff.lst*
must be sorted with
sort(1)
before executing
**coeff**.

OpenBSD 6.6 - September 9, 2014
