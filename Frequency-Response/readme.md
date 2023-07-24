# Chapter 5: Frequency Response and SID

<p align="center"><img src="/Frequency-Response/pics/1.jpg?raw=true" width="720px" /></p>

When designing and assessing a power amplifier, one of the most crucial characteristics we need to pay attention to is its frequency response. The frequency response should ideally encompass the range of human hearing, which is generally accepted to be from 20 Hz to 20 kHz. However, the way our ears perceive different frequencies is not linear. For example, we are more sensitive to frequencies between 2 kHz to 4 kHz, where the human voice resides, and less sensitive to very high or very low frequencies.

Despite this non-linear perception of ours, as audio power amplifier designers, our primary task is to ensure a flat frequency response. In other words, our amplifier should not favor or attenuate any particular frequency within the range of human hearing. That's the job of equalizers, or rather, the composers and producers who are conscientious about their music's tonal qualities.

## The role of slew-rate and why 20Hz to 20KHz is not enough
The slew rate is essentially how quickly an amplifier can respond to changes in the input signal. It's often measured in volts per microsecond (V/µs). So if an amplifier has a slew rate of 10 V/µs, it means the output can change by up to 10 volts in a single microsecond. Regardless of those details, as a general rule: higher the slew rate, higher the ability of amplifier to represent high frequency components.

Now let's talk about what happens if the slew rate is too slow. If an amplifier's slew rate can't keep up with the rapid changes in the input signal, it won't accurately reproduce the sound. This effect is called **slew-induced distortion (SID)**. When it happens, the high-frequency components of the sound can get "smudged" into the lower frequencies. This smudging can color the sound, meaning it can add unwanted tonal qualities to the music.

For an obvious example, imagine a very slow slew amplifier, in which the frequencies that are produced by a violin are smudged into the frequency range of a cello due to slew-induced distortion, you might mistakenly think there's a cello playing in the background even though there isn't. 

In a similar manner, that capping the frequency response at 20 kHz isn't sufficient. The concept of slew-induced distortion comes into play here. This distortion occurs when an amplifier cannot keep up with the rate of change of the input signal. If the amplifier's frequency response is not wide enough, the harmonics of high-frequency components (which themselves are beyond our hearing) could "fold back" into the audible range due to the limited slew rate of the amplifier. This distortion results in a coloration of sound, affecting the accuracy of the audio reproduction.

By ensuring a wide frequency response, we can minimize this distortion and provide a sound that is true to the original input signal, devoid of any unwanted coloration or alteration. That's why, in practice, a good power amplifier should have a frequency response extending significantly beyond the limits of human hearing, often up to 80 kHz or more. This ensures an ample margin to prevent audible slew-induced distortion and provides the listener with a pristine and accurate sound experience.

## High frequency response is good, as long as it's not *too* high

While a wide frequency response is beneficial for accurate sound reproduction, it's important to remember that there's an optimal range for this parameter. You might be tempted to think that if a 100kHz bandwidth is good, a 300kHz or even higher bandwidth would be even better. However, this is not necessarily the case.

It turns out that designing an amplifier to have an excessively high bandwidth can actually introduce more problems than it solves. This is due to a phenomenon called "oscillation." In electronics, an oscillator is a circuit that produces a repetitive signal. Normally, this is a useful device, but unintentional oscillation in an amplifier can be a serious problem.

When an amplifier has a very high bandwidth, it's essentially more sensitive to high-frequency signals. This sensitivity can lead to a situation where the amplifier picks up and amplifies noise or other unintended signals. In the worst-case scenario, it might even start to amplify its own output signal, creating a feedback loop that results in oscillation. These oscillations can cause the amplifier to become unstable and can lead to distortion, reduced sound quality, and potentially even damage to the amplifier.

Moreover, in real-world scenarios, other factors like the amplifier’s internal layout, the parasitic inductance, and capacitance can result in unintentional oscillations at high frequencies.

Finally, very high-frequency signals are more prone to radiate from the speaker cables, effectively turning them into an antenna and potentially causing interference with other electronic devices.

So, while a wide frequency response is a good thing, it's essential to have a balanced approach. The aim should be to cover the entire audio spectrum and a bit beyond, but not to excessively extend into very high frequencies.

## What about low frequencies?

The low-frequency response of an audio power amplifier is another aspect that demands attention. While human hearing is typically limited to frequencies as low as 20Hz, there is an argument that frequencies lower than this can be "felt" rather than heard. This applies to frequencies down to about 5Hz, especially in the context of certain genres of music and in cinema sound effects where the emphasis is on creating an immersive sensory experience.

However, it's worth noting that if the low-frequency response extends all the way down to DC (0Hz), it can introduce some potential problems. Preamps in modern audio systems are capable of representing frequencies down to DC, but if these extremely low frequencies are not adequately filtered out, they can lead to unintended activation of the speaker's protection circuitry.

Why is this a problem? A speaker's protection circuit is designed to prevent damage to the speaker from excessively high power levels. If this circuit is triggered by very low-frequency signals (or DC signals), it can lead to various kinds of noise such as popping sounds, and can even cause interruptions in the audio.

The solution to this issue is to use a technique known as capacitive coupling. This essentially involves using a capacitor (C) and a resistor (R) to form an RC filter at the input stage of the amplifier. The RC filter serves to block DC and very low-frequency signals, while allowing higher-frequency signals to pass. This is why it's sometimes also referred to as a "high-pass" filter.

In practical terms, you would typically choose a cutoff frequency for this high-pass filter that is just below the audible range, such as 3Hz. This ensures that all audible frequencies (and a bit beyond) are faithfully reproduced, while potentially problematic ultra-low frequencies and DC are effectively filtered out. This way, we maintain the integrity of the audio signal and ensure the smooth operation of the amplifier and speaker system.