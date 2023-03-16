


![Logo](https://github.com/Sheikh-Araf/SoundFilter/blob/main/Resources/SoundFilter_resources/icon_48.png) 
# Sound Filter 

This software is designed to analyze sound frequencies and separate mixed sounds into two distinct tracks. By determining the frequency response of a given sound and mixed sound, it can design a filter that isolates the two original sounds.

# Theory Implementation

**Frequency Response**: The frequency response is the quantitative measure of the output spectrum of a system or device in response to a stimulus. In this software, the frequency response is used to determine the frequencies of the original sounds and the mixed sound.

**Bilinear Transformation**: The Bilinear transform is a mathematical relationship which can be used to convert the transfer function of a particular filter in the complex Laplace domain into the z-domain, and vice-versa. The bilinear transform is the result of a numerical integration of the analog transfer function into the digital domain. The software uses the Bilinear transform to design a filter that can isolate the two original sounds.

![equation1](https://github.com/Sheikh-Araf/SoundFilter/blob/main/images/equation1.png)

**Low Pass and High Pass Filters**: A high-pass filter (HPF) attenuates content below a cutoff frequency, allowing higher frequencies to pass through the filter. A low-pass filter (LPF) attenuates content above a cutoff frequency, allowing lower frequencies to pass through the filter. The software uses both low-pass and high-pass filters to separate the mixed sound into its original components.


## How To Use

**Step 1:** First clone the repository

```bash
  git clone https://github.com/Sheikh-Araf/SoundFilter.git
```
**Step 2:** Open MATLAB Software 

**Step 3:** File > Open

**Step 4:** Choose the ```home/user-name/SoundFilter/src/SoundFilter.mlapp```




## Demo

To demonstrate the functionality of this software, we will use a sample siren sound that has been combined with an unknown sound. Our objective is to design a filter that will separate the siren sound and produce two separate audio sounds.

**Sample Input**

The input signal consists of a siren sound and an unknown sound, as shown in the following screenshot:

![input](https://github.com/Sheikh-Araf/SoundFilter/blob/main/images/input.png)

The frequency ranges of the unknown sound in the combined signal are between 500 Hz and 2000 Hz.



**Filter Design**

To separate the siren sound from the combined signal, we will use the Bilinear transformation method to design a filter that transforms a low-pass filter into a high-pass filter.

The filter order will be 3rd, and the cut-off frequency of the filter will be set to 1000 Hz.

**Output**

After applying the filter to the input signal, we obtain the following two separate audio sounds:

**Siren sound:**

![output1](https://github.com/Sheikh-Araf/SoundFilter/blob/main/images/demo1.png)

**Separated sound:**

![output2](https://github.com/Sheikh-Araf/SoundFilter/blob/main/images/demo2.png)
## License

[MIT](https://raw.githubusercontent.com/Sheikh-Araf/SoundFilter/main/LICENSE)

