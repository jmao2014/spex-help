Spectral Fitting
================

To infer relevant physical parameters from observed X-ray spectra,
physical models are needed. The models need to calculate the expected
X-ray spectrum based on physical parameters, like the electron
temperature, emission measure and density distributions, ion and
elemental abundances, mass motions, and the nature of the ambient
radiation field. Unfortunately, the physical models cannot be compared
directly to the measured spectra, because the instruments used to obtain
the spectra change the spectrum for example by adding background
components (instrument noise), change the continuum shape due to the
sensitivity of the mirror (effective area), and blur spectral lines due
to the instruments spectral resolution.

To take these instrumental components into account, the usual procedure
is to apply a forward modelling technique by convolving theoretical
model spectra with the instrumental response and to vary the model
parameters in order to optimize the fit of the model to the
observational data. A common approach is to consider first a simplified
plasma model for the X-ray source, neglecting much of the complexity of
the temperature and density structure and of the effects of opacity, and
to synthesize such models into successively more sophisticated
approximations of the source model.

.. _label: fig:1
.. figure:: trpb01.png
   :alt: Processing Flow Diagram for Spectral Modelling of optically thin plasmas (from Mewe 1992).
   :width: 80.0%

In Figure `1 <#fig:1>`__ we give in a processing flow diagram
schematically the process of spectral modelling for the case of
optically thin coronal plasmas. The synthetic spectra program is fed
with input parameters from the spectral model (atomic data for
ionization and line and continuum excitation), the instrumental model,
and from the assumed plasma model for the source. The synthetic spectra
code generates spectra which can be compared to the observations and
tested by means of statistical fitting procedures.
