# Group 4 - Tempo Estimation
## Features used  
For plotting:
- RMS energy
- Onsets

For estimating a tempo:
- RMS energy
- Periodicity analysis (autocorrelation of energy derivative)  

## Signal Flow
1. Input signal
2. Find RMS energy of signal
3. Find derivative of RMSE
4. Take only positive values to evaluate onsets
5. Autocorrelate derivative for periodicity analysis
6. Take only autocorrelation above a threshold
7. Find time difference values at strong AC values
8. Filter possible time difference values
9. Convert to tempo

## Future Improvments
Use spectral features to determine the genre of the song and set a range for estimating the tempo.
Determine the best autocorrelation threshold for different genres of music
