# cyclostationary 

Implementation of cyclostationary analysis:

requirements.txt - dependencies\
analysis/src/audiosample.npy  - sample array to verify computation\
analysis/src/cyclostationary.py - estimates Spectral Correlation Density (SCD) using FFT accumulation (FAM) method\
analysis/src/livescd.py       - reads from microphone and plots scd using pyqtgraph\
analysis/src/intro.ipynb      - jupyter notebook showing SCD for different modulation types\
analysis/gen/bpsk.py          - generate bpsk file\
analysis/gen/noise_bpsk.npy   - generated by gen/bpsk.py

To verify: 
~~~
python cyclostationary.py # should print "audiotest: PASS (error=0.0)" and show
~~~

![Screen shot](analysis/images/ScreenShot_scf_fam.png)

To acquire audio from microphone and plot scf:
~~~
python livescd.py
~~~

![Screen shot](analysis/images/ScreenShot_livescf.png)
