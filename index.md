# Introduction

This is the demo page of our paper submitted to ICLR 2026.

### Examples of Non-blind test set of the URGENT 2025 Challenge:
Note: 
1. We provide examples for multiple languages.

2. The difference between Early Reflected and Shifted Anechoic speech training targets is noticeable only when the input noisy speech contains reverberation.

3. The effect of the GAN correction is typically audible only under **severe** degradations (e.g., low SNR, packet loss, bandwidth extension, etc.).


### Example1:

**Noisy (noise, codec, reverb):**

<audio style="width:320px" controls="controls">
	<source src="wavs/noisy_18.flac" type="audio/wav" />
</audio>

**Early-reflected:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early_18.flac" type="audio/wav" />
</audio>

**Early-reflected + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early+GAN_18.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted_18.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted+GAN_18.flac" type="audio/wav" />
</audio>

-----------------------------------------------------------
### Example2:

**Noisy  (noise, codec, reverb):**

<audio style="width:320px" controls="controls">
	<source src="wavs/noisy_320.flac" type="audio/wav" />
</audio>

**Early-reflected:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early_320.flac" type="audio/wav" />
</audio>

**Early-reflected + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early+GAN_320.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted_320.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted+GAN_320.flac" type="audio/wav" />
</audio>

-----------------------------------------------------------
### Example3:

**Noisy (noise, packet loss, reverb):**

<audio style="width:320px" controls="controls">
	<source src="wavs/noisy_344.flac" type="audio/wav" />
</audio>

**Early-reflected:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early_344.flac" type="audio/wav" />
</audio>

**Early-reflected + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early+GAN_344.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted_344.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted+GAN_344.flac" type="audio/wav" />
</audio>

-----------------------------------------------------------
### Example4:

**Noisy (noise, packet loss, clipping):**

<audio style="width:320px" controls="controls">
	<source src="wavs/noisy_824.flac" type="audio/wav" />
</audio>

**Early-reflected:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early_824.flac" type="audio/wav" />
</audio>

**Early-reflected + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/early+GAN_824.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted_824.flac" type="audio/wav" />
</audio>

**Shifted anechoic clean + GAN:**

<audio style="width:320px" controls="controls">
	<source src="wavs/shifted+GAN_824.flac" type="audio/wav" />
</audio>

-----------------------------------------------------------

### Examples of our speech enhancement model applied to real noisy speech:


**Example 1: [Jensen's speech](https://www.youtube.com/watch?v=zbzCiau3hWc&t=24s)**

<img src="img/Jensen.png" style="width:30%; height:auto;"/>


**Original input (noisy, highly-reverb, bandwidth-limitation (16kHz))**:

<audio style="width:320px" controls="controls">
	<source src="wavs/Run_noisy.wav" type="audio/wav" />
</audio>

**Enhanced:** 

<audio style="width:320px" controls="controls">
	<source src="wavs/Run.wav" type="audio/wav" />
</audio>

**Enhanced and bandwidth extension to 32k:**  

<audio style="width:320px" controls="controls">
	<source src="wavs/Run_32k_kaiser_best.flac" type="audio/wav" />
</audio>

-----------------------------------------------------------

**Example 2: [Einstein's speech](https://history.aip.org/exhibits/einstein/voice3.htm)**

<img src="img/Einstein.jpg" style="width:30%; height:auto;"/>

**transcript: Large parts of the world are faced with starvation, while others are living in abundance.**  	

**Original input (noisy, clipping, mp3 artifact, bandwidth-limitation (8kHz))**:

<audio style="width:320px" controls="controls">
	<source src="wavs/Einstein_mp3_8k_noisy.wav" type="audio/wav" />
</audio>

**Enhanced:** 

<audio style="width:320px" controls="controls">
	<source src="wavs/Einstein_mp3_8k.wav" type="audio/wav" />
</audio>

**Enhanced and bandwidth extension to 16k:**  

<audio style="width:320px" controls="controls">
	<source src="wavs/Einstein_mp3_8k_16k.wav" type="audio/wav" />
</audio>

-----------------------------------------------------------

**Example 3: [Apollo 11 astronaut Neil Armstrong gives his classic confirmation of the first footsteps on the moon](https://science.nasa.gov/resource/sounds-of-mars-one-small-step/)**

<img src="img/Apollo.png" style="width:30%; height:auto;"/>

**transcript: One small step for (a) man, one giant leap for mankind.**  	

**Original input (noisy, bandwidth-limitation)**:

<audio style="width:320px" controls="controls">
	<source src="wavs/sounds-of-mars-one-small-step-earth_noisy.wav" type="audio/wav" />
</audio>


**Enhanced and bandwidth extension to 16k:**  

<audio style="width:320px" controls="controls">
	<source src="wavs/sounds-of-mars-one-small-step-earth_8kto16k.wav" type="audio/wav" />
</audio>

-----------------------------------------------------------

**Example 4: [Harry Potter and the Philosopher's Stone](https://youtu.be/ibRcSCRAyTA?t=22) (2001)**

<img src="img/Potter.png" style="width:30%; height:auto;"/>

**Original input (noisy (music), bandwidth-limitation (16kHz))**:

<audio style="width:320px" controls="controls">
	<source src="wavs/Potter_noisy.wav" type="audio/wav" />
</audio>

**Enhanced:** 

<audio style="width:320px" controls="controls">
	<source src="wavs/Potter.wav" type="audio/wav" />
</audio>

**Enhanced and bandwidth extension to 32k:**  

<audio style="width:320px" controls="controls">
	<source src="wavs/Potter_32k.wav" type="audio/wav" />
</audio>

-----------------------------------------------------------

**Example 5: [Airport announcements](https://www.youtube.com/watch?v=7y9asDUhwTc)**

<img src="img/airport.png" style="width:30%; height:auto;"/>


**Original input (noisy, highly-reverb, multi-lingual, TTS speech)**:

<audio style="width:320px" controls="controls">
	<source src="wavs/airport_noisy.wav" type="audio/wav" />
</audio>




| Team            | DNSMOS | NISQA | UTMOS | PESQ | ESTOI | SDR   | MCD  | LSD  | SBERT | LPS  | SpkSim | CAcc  | Overall ranking score|
|-------------------|--------|-------|-------|------|--------|-------|------|------|--------|------|---------|--------|--------------|
| Bobbsun| 3.01 (8) |	3.41 (6) |	2.4 (3)	|2.95 (1)	|0.86 (1)	|14.33 (1)	|3.01 (4)	|2.83 (5)	|0.91 (1) |	0.86 (1) |	0.85 (1) |	88.92(1) | 2.52 (1)|
| Our GAN correction| 3.04 (5) |	3.53 (3) |	2.3 (6)	| 2.78 (4)	0.84 (4)	| 12.25 (5)	| 2.97 (3) |	2.75 (4)	| 0.9 (2)	| 0.84 (3) |	0.85 (1)	|88.13 (2)	|3.17 (2)|
| 3.00   | 3.45  | 2.31  | 2.74 | 0.84   | **13.06** | 3.30 | 3.08 | 0.89   | 0.84 | 0.83    | 87.94 |
| rc |3.01 (8) |	3.21 (9)	|2.3 (6)	|2.79 (3)	|0.85 (2)	|13.11 (2)	|2.93 (2) |	2.94 (8) |	0.9 (2) |	0.85 (2) |	0.84 (3) |	88.05 (3) |	4.02 (3)|
| Our Early reflected| 3.06 (4) |	3.23 (8)	|2.26 (8)	|2.81 (2)	|0.85 (2)	|12.28 (4) |	2.87 (1)	|2.66 (1)	|0.9 (2)	|0.84 (3)	|0.82 (5)	|87.62 (5)	|4.04 (3)|

**Enhanced:** 

<audio style="width:320px" controls="controls">
	<source src="wavs/airport.wav" type="audio/wav" />
</audio>
