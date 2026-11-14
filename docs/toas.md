# Times of arrival

Pulse times of arrival (TOAs) measured from our MeerKAT observations up to the end of June 2026.
Later observations will be added in future updates.

!!! warning "Preliminary"
    These TOAs are preliminary and may be revised as the analysis improves.
    Please [get in touch](contact.md) before using them in a publication.

## Downloads

| File | Contents |
|---|---|
| [all_toas.csv](data/toas/all_toas.csv) | All TOAs below, with peak flux density and pulse width |
| [GLEAMXJ0704.tim](data/toas/GLEAMXJ0704.tim) | GLEAM-X J0704−37 (tempo2 / PINT format) |
| [ASKAPJ1839.tim](data/toas/ASKAPJ1839.tim) | ASKAP J1839−0756 |

## How the TOAs were measured

- **Data:** dynamic spectra made from the MeerKAT visibilities at the source position (UHF band),
  at 8 s time resolution.
- **TOA:** the centre of a Gaussian fitted to the band-averaged Stokes I light curve. When pulses overlap,
  they are fitted together. The error is the 1σ uncertainty on the fitted centre.
- **Time system:** topocentric UTC at MeerKAT. The TOAs are **not** barycentred and **not** corrected for
  dispersion. In the `.tim` files the site code is `meerkat` and the frequency is the band centre (816 MHz).
- **Multiple pulses:** observations with more than one pulse, or a pulse with several components, have one
  TOA per component.

## All TOAs

{{ read_csv('data/toas/all_toas.csv', dtype='str', keep_default_na=False, disable_numparse=True) }}
