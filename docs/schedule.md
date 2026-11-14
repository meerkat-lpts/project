# Completed observations

MeerKAT observations taken so far for this project. All observations are imaged and also recorded
with the PTUSE beamformer (search mode, full polarisation) for high time resolution.
The table lists the time on source for each target.

**Bands:** UHF = 544–1088 MHz; L-band = 856–1712 MHz.

{{ read_csv('data/schedule.csv', dtype='str', keep_default_na=False, disable_numparse=True) }}

The table is also available as a [CSV file](data/schedule.csv).

!!! note "Errored observation"
    The observation of ASKAP/DART J1832−0911 and ASKAP J1839−0756 on 2026-09-28 is not listed above:
    its timing was offset from the predicted pulse arrival times, so the pulses fell outside the observation.
