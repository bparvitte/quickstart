+++
title = "Test self publi"
date = 2021-06-09T00:00:00+02:00
draft = false
+++

### Introduction {#introduction}

Infrared heterodyne spectrometers have been successfully used for astronomical
and geophysical applications (([Betz et al. 1976](#orgccfa21f); [Betz 1981](#org4784f5e); [Kostiuk et al. 1976](#orgbbee88c); [Kostiuk, Hillman, and Faris 1981](#orgb11e21e))). The Reims GSMA laboratory has developed
for several years high resolution heterodyne receivers for atmospheric ozone
studies. The local oscillator was a \ce{CO2} laser and the spectral range was about
1.5 GHz.

The development of a wider band heterodyne receiver has many
advantages. First, it enables us to study lines which were out of range of the
first apparatus. For the same reason, we use now either a \ce{<sup>12</sup>C<sup>16</sup>O2} or
a \ce{<sup>12</sup>C<sup>18</sup>O2}, laser as local oscillator. We also need this wide band
spectrometer for recording ground-based atmospheric absorption spectra. For
those spectra, the sun is used as a source and the absorption by the low
altitude layers is very wide : because of the pressure broadening. In order to obtain the 100% transmission, we must record the whole line profile. A 2 GHz scan is, at least necessary to fulfill this condition.


### Heterodyne spectrometer : description {#heterodyne-spectrometer-description}

In order to obtain a 2.5 GHz bandwidth, three main elements with this bandwidth
must be associated :

-   A fast photodiode which acts as an optical mixer
-   Low noise, wide band amplifiers, in order to work at a sufficient level
-   RF analysis and detection system.

A short description of these elements and of the data acquisitions System follows
below.


#### Optical part {#optical-part}

This part has been previously described, and so only a short description
necessary for the understanding of this work will be given here (([Thiébeaux et al. 1988](#org37dc24d); [Courtois, Thiébeaux, and Delahaigue 1984](#org79ba81e))).
The beams of the local oscillator and of two thermal sources are focused
onto a photodiode, which acts as an infrared mixer.
The photodiode is one of the most important element of the spectrometer. The
bandwidth of the apparatus is generally limited by the diode bandwidth.
Therefore the choice of this element is particularly important. We use a reverse-
biased, fast HgCdTe photodiode from S.A.T. (Société Anonyme de
Télécommunications, France). This mixer is set in a down-looking special
laboratory made Dewar. All connections are made by using as short as possible
coaxial cables. It works at liquid nitrogen temperature\_ The bandwidth is about
3 GHz for a bias between 1.3 and 2 Volts.
Our set-up is a double beam heterodyne system. The two thermal beams are chopped
at different frequencies. High precision mechanical choppers (EG&G model 197)
are used. One of the beam is for reference and the other for measurement.
Transmission is proportional to the ratio of the two signals. This technique
suppresses low frequency drift of the spectrometer. For laboratory
studies, an absorption cell is put on the second beam. For atmospheric studies, the
measurement beam is obtained with a sun tracker (([Delahaigue et al. 1988](#org061f075))).


#### Radio frequency analysis {#radio-frequency-analysis}

We first use two wide band and low noise preamplifiers which were specially
studied for this experiment (Micronic - France). The first one has an incorporated bias tee.
Their characteristics are :

-   70 dB total gain
-   2.5 dB noise
-   12.7 GHz bandwidth.

This amplification allows the analyzer to work at sufficient level.
The analyzer is heterodyne type. It uses an RF mixer, a fixed filter and a local
oscillator (see figure [fig:1](#fig:1)). The mixer works as following " for an input
\\(\nu\_{RF}\\) frequency signal and a \\(\nu\_{LO}\\) frequency local oscillator signal,
the output signal frequency is equal to \\(\nu\_{IF}=\\|\nu\_{RF}-\nu\_{LO}\\|\\). With a
filter centered at \\(f\_{IF}\\), the analysis of the RF signal between 0 and
\\(f\_{IF}\\) is obtained by sweeping the local oscillator frequency
from \\(f\_{IF}\\) to  \\(2 \times  f\_{IF}\\). The resolution of the RF analyzer is then
equal to the bandwidth B of the filter.
The RF local oscillator is a Marconi 2042 synthesizer. It works between 10 kHz
and 5.4GHz. Frequency and output level accuracies are widely sufficient for our
experiment. The maximum frequency 5.4 GHz value leads to the choice of a 2.7 GHz
filter. This synthesizer is completely controlled by a micro-computer via IEEE
port.
Several RF mixers were tested in order to obtain the best results. It was
difficult to find a mixer which had sufficient bandwidth on the three ports (IF, RF,
LO). We finally decided to use the Anzac MDC 154 (IF 0.1 - 3000 MHz, RF, LO 0.3- 5 GHz). The upper limit of the mixer on the LO port is slightly to low.
The last part of the analyzer is composed of a selective amplifier centered at 2.7
GHz (Micronic) and a four sections cavity filter (Trilithic 2.7 GHz, 10 MHz). The
detection of the RF signal is done by a RF diode Texscan CD51 operated in the
square-law mode. This type of analyzer has several advantages. The apparatus
function is well known and given by the filter response. The resolution is equal to
the width of this response. With a 10 MHz filter, the resolution is at least 5 times
lower than the Doppler line width of the studied molecules.

{{< figure src="/ox-hugo/1995ParvitteIJIMWafig1.png" caption="Figure 1: Scheme of the RF analyzer <a name=\"fig:1\"></a>" >}}


#### Data acquisition {#data-acquisition}

The RF diode gives a signal proportional to the incident power on the of
photodetector. We use two lock-in amplifiers (model EGG 5301) to discriminate
the reference and measurement signals. Each one is adjusted on the modulation
frequency of one of the thermal beams. The lock-in amplifiers are used with a
time constant \\(\tau\\) equal to 100 ms and a rollof rate of 12 dB/Oct. The DC output
signals between 0 and 10 volts are then digitized. In order to have high dynamic
and high resolution, we use for each channel a voltage to frequency converter (0 -
10 Volts, 10 MHz) and a counter. The numerical integration is controlled by an
accurate 4MHz quartz oscillator. The integration time is generally about 1 to 10
seconds. Pressure and temperature in the gas cell arc simultaneously recorded.
The laboratoy developed software controls data acquisition and the local oscillator
frequency. Parameters such as frequency step of the LO, number of steps,
integration time are fixed with the computer. We can either record single
spectra or accumulate them. The system speed is only limited by file response
time of the synthesizer which is IEEE controlled. The results of the
measurements are directly visualized on the screen of the computer.


### Results {#results}


#### Test of the photomixer {#test-of-the-photomixer}

Many methods for measuring the bandwidth of a photodetector areavailable. The
best known is the measure of the noise spectrum of the detector when it is
illuminated by a laser. Another consists in recording the beat signal of a local
oscillator beam and a frequency-shifted beam. The shifted beam is often obtained
by using all acousto-optic modulator (([Vérié and Sirieix 1972](#org0b50e2d))). As tunable diode
lasers emitting in the 10 µm region are available in our laboratory., we decided
to use the TDL's beam as the frequency-shifted beam. In this case, the radiation
of the \ce{CO2} laser and of the TDL are superimposed on the HgCdTe photodiode.
The frequency of the signal is then equal to the difference between the \ce{CO2}
laser line frequency and the TDL frequency.
For a fixed value of the injection current of the diode, the spectral width of
this signal can be measured and is about 50 MHz. This value is negligible in
comparison with the total bandwidth of the detector. The beat signal is recorded
for different value of the diode frequency. This measurement gives a good
description of the photomixer response. The two following conditions are
required : the diode emission must be monomode and there must be no mode hop on an
interval greater than the double of the bandwidth around the frequency of the
\ce{CO2} laser line.
The diodes we use are PbSnSe diodes: working between 20 and 40 K. They are Set
in a closed-cycle helium cooler. The cooler and the current driver are from
Mütek (Germany). The diode is operated in a multilongitudinal mode. A grating monochromator selects one mode.
The frequency of the diode is swept around the \ce{CO2} laser line frequency by tuning
the injection current. The fringes of a spherical Fabry-Perot are simultaneously
recorded so we could have a relative scale frequency versus injection current.
The confocal etalon is a 25 cm one with an invar structure. It takes place in a vacuum
cell and its sharpness is about 40 when illuminated by a well stabilized
\ce{CO2} laser. The free spectral range is 0.01 cm-1.
Measurements have been done near the 9P20 line of \ce{<sup>12</sup>CO2} laser (1046.85 cm-1). Figure [fig:2](#fig:2) shows an example of measurement.
It has been obtained with the infrared mixer and the preamplifiers. The frequency scale is in megahertz
and the signal scale is linear.
The total width of the signal is approximately of 0.185 cm-1. This value correspond to a bandwidth of 2.7 MHz.
The receiver's bandwidth is therefore limited by the amplifiers bandwidth.
The peak is obtained when the diode frequency is close to the laser line
frequency. It seems to be due to a peak response of the preamplifiers
for low frequency (< 50 MHz).

</ox-hugo/1995ParvitteIJIMWafig2.pdf>


#### First spectra {#first-spectra}

In order to check this new apparatus, we decided to record an absorption
line shifted from more than 2 GHz from the local oscillator.
The Ammonia molecule seems to be a good choice for these tests.
The research of coincidences between \ce{NH3} and the \ce{CO2} laser lines in the Hitran
Datatabase (([Rothman et al. 1992](#org96b82f9))) leads to only a few possibilities. We chose to record the \ce{NH3}
R(5,1) line near 9 µm  (see Table [tab:1](#tab:1)). The line's center is shifted from - 2343 MHz
from the 9P10 \ce{CO2} laser line. As we need at least 200 MHz on both sides to
record the whole line profile, this line is at the limit of the 2.5 GHz heterodyne
receiver.
We present in figure 3 one of the recorded spectra. It has been recorded with
approximately 2 torrs of \ce{NH3} and a path length of 1.60 meter.
The characteristics are:

-   200 points
-   3 MHz steps
-   10 s for each point (total time: 35 min.).

The most important element we can see on this spectrum is that the line position is
slightly different from the expected value. The line center is found at - 2100 MHz
&plusmn; 5 MHz from the 9P10 \ce{CO2}\_laser line. (Table [tab:2](#tab:2)).This value is coherent with
previous measurements (([Sasada et al. 1986](#orga24e82d))).

<div class="table-caption">
  <span class="table-number">Table 1</span>:
  Position and intensity of the R(5,1) line of Ammonia (Hitran database 1992) <div id="tab:1"></div>
</div>

| frequency | intensity         |
|-----------|-------------------|
| (cm-1)    | (cm-2/(mol.cm-1)) |
| 1055.5470 | 9.33E-22          |

<div class="table-caption">
  <span class="table-number">Table 2</span>:
  Position of the R (5 1) line of \ce{NH3} <div id="tab:2"></div>
</div>

| Source                               | wave number | shift withthe 9P 10line of \ce{CO2} |
|--------------------------------------|-------------|-------------------------------------|
|                                      | (cm 1)      | (MHz)                               |
| ([Rothman et al. 1992](#org96b82f9)) | 1055.5470   | -2343                               |
| ([Sasada et al. 1986](#orga24e82d))  | 1055.5540   | -2130                               |
| This work                            | 1055.5550   | -2100                               |

</ox-hugo/1995ParvitteIJIMWafig3.pdf>


### Conclusion {#conclusion}

A double beam heterodyne spectrometer with 2.5 GHz bandwidth was built in Reims.
The receiver's bandwidth was measured by heterodyning radiation from a \ce{CO2},laser with the radiation from a tunable diode laser.
The spectrometer was used for laboratory studies. Ammonia absorption spectra were recorded. Line positions in agreement with other works were measured.
This apparatus will soon be used for atmospheric ozone studies in
association with an isotopic \ce{<sup>12</sup>C<sup>18</sup>O\_2} laser to avoid atmospheric
\ce{CO2} absorption.


## Bibliography {#bibliography}

<a id="org4784f5e"></a>Betz, Albert L. 1981. “Ethylene in IRC+ 10216.” _The Astrophysical Journal_ 244:L103–5.

<a id="orgccfa21f"></a>Betz, Albert L., M. A. Johnson, Robert A. McLaren, and Edmund C. Sutton. 1976. “Heterodyne Detection of CO2 Emission Lines and Wind Velocities in the Atmosphere of Venus.” _The Astrophysical Journal_ 208. AA(California, University, Berkeley, Calif.), AB(California, University, Berkeley, Calif.), AC(California, University, Berkeley, Calif.):L141.

<a id="org79ba81e"></a>Courtois, Daniel, Claude Thiébeaux, and Alain Delahaigue. 1984. “Heterodyne Spectrometer for the 10 Micron Region.” _International Journal of Infrared and Millimeter Waves_ 5:185–95.

<a id="org061f075"></a>Delahaigue, Alain, Claude Thiébeaux, Daniel Courtois, and Hervé Le Corre. 1988. “Design of a Sun Tracker for a Laser Heterodyne Spectrometer.” _Infrared Physics_ 28 (1):1–6.

<a id="orgb11e21e"></a>Kostiuk, Theodor, John J. Hillman, and James L. Faris. 1981. “Precision Heterodyne Measurements of Ozone Spectral Lines Near 9.5 ΜM.” _Journal of Molecular Spectroscopy_ 89 (2). Elsevier:397–404.

<a id="orgbbee88c"></a>Kostiuk, Theodor, Michael J. Mumma, Michael M. Abbas, and David Buhl. 1976. “Sensitivity of an Astronomical Infrared Heterodyne Spectrometer.” _Infrared Physics_ 16:61–64.

<a id="org96b82f9"></a>Rothman, Laurence S., Robert R. Gamache, Richard H. Tipping, Curtis P. Rinsland, Mary Ann H. Smith, D. Chris Benner, Vidya Malathy Devi, et al. 1992. “The HITRAN Molecular Database: Editions of 1991 and 1992.” _Journal of Quantitative Spectroscopy and Radiative Transfer_ 48 (5-6):469–507.

<a id="orga24e82d"></a>Sasada, Hiroyuki, R.H. Schwendeman, Gottfried Magerl, Robert L. Poynter, and Jack S. Margolis. 1986. “High-Resolution Spectroscopy of the V2 = 2 a ← V2 = 1 S Band of 14NH3.” _Journal of Molecular Spectroscopy_ 117 (2). Elsevier BV:317–30. <http://dx.doi.org/10.1016/0022-2852(86)>90157-8.

<a id="org37dc24d"></a>Thiébeaux, Claude, Daniel Courtois, Alain Delahaigue, Hervé Le Corre, Jean-Claude Mouanda, and André Fayt. 1988. “Dual-Beam Laser Heterodyne Spectrometer Ethylene Absorption Spectrum in the 10 Μm Range.” _Applied Physics B: Photophysics and Laser Chemistry_ B47:313–18.

<a id="org0b50e2d"></a>Vérié, Christian, and Michel B. Sirieix. 1972. “Gigahertz Cutoff Frequency Capabilities of CdHgTe Photovoltaic Detectors at 10.6 Μ.” _IEEE Journal of Quantum Electronics_ 8 (2):180–84.
