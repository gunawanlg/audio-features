# audio-features
An attempt to standardize all audio features `python` library.

## MFCC
Compares different python library on how to create common speech 39 MFCC features which decomposed to:
* 12 MFCC features, here the first "DC component" of MFCC is removed + 1 log-energy appended (13 total)
* 13 Delta MFCC features and log-energy, 1st order difference by time
* 13 Delta-Delta MFCC Features and log-energy, 2nd order difference by time
* 25 ms windows length, with 10 ms window step
* no window, this equal to square windows which can be created using np.ones(nfft)

![MFCC Comparison](https://github.com/gunawanlg/audio-features/blob/master/assets/MFCC%20Compare.png)
